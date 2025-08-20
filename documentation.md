---
marp: true
theme: custom-theme
paginate: true
header: 'Product Documentation: API v2.0'
footer: '© 2025 Software Corp.'
---

<!--
theme: custom-theme
class:
 - lead
-->

<style>
  /* Define a custom theme for the presentation */
  @theme custom-theme {
    section {
      background-color: #f0f4f8;
      color: #333;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }
    h1, h2 {
      color: #005a9c;
      border-bottom: 2px solid #005a9c;
    }
    code {
      background-color: #e0e8f0;
      border-radius: 4px;
      padding: 2px 6px;
    }
    a {
      color: #0078d4;
    }
  }
</style>

# **Product Documentation: API v2.0**
A Guide for Developers

---

## Agenda

1.  Introduction to API v2.0
2.  Key Features & Endpoints
3.  Authentication
4.  Algorithmic Complexity
5.  Q&A

*Contact for support: <a href="mailto:22f1001519@ds.study.iitm.ac.in">22f1001519@ds.study.iitm.ac.in</a>*

---

<!--
_class:
 - invert
backgroundImage: "url('api-background.jpg')"
backgroundSize: cover
-->

## Key Features

- **RESTful Architecture**: Predictable, resource-oriented URLs.
- **JSON-based**: Standard JSON for requests and responses.
- **OAuth 2.0**: Secure and standardized authentication.
- **Scalable Infrastructure**: Built for high-throughput.

---

<!--
_header: ''
_footer: ''
-->

## Algorithmic Complexity

Understanding the performance of our core algorithms is crucial. The primary search endpoint has the following complexity:

$$
O(n \log n)
$$

Where $n$ is the number of records in the dataset. This ensures efficient performance even as data scales.

---

## Authentication Flow

Our API uses the OAuth 2.0 Client Credentials flow.

1.  **Request Token**: Your application sends its `client_id` and `client_secret` to the `/oauth/token` endpoint.
2.  **Receive Token**: The server validates credentials and returns a temporary `access_token`.
3.  **Access API**: Include the `access_token` in the `Authorization` header for all subsequent API calls.
