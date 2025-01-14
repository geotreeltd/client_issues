---
name: API Issue
about: Report an issue with the API
title: ""
labels: ""
assignees: ""
---

**How were you calling the API**

- Caller: [e.g. Curl, Postman, Python]

**Inputs**
Paste the http input. Put asterixes instead of any sensitive information such as API keys

e.g.

```http
    POST https://api.geotree.com/client/users/save HTTP/1.1
    Accept: application/json
    Content-Type: application/json
    X-ML-Token: bearer ***********************************

    {
        "newUsers":[ {
            "email": "tony@mantle-labs.com",
            "first_name": "Tony",
            "last_name": "Kimani",
            "role":"admin"
        }
        ]
    }
```

**Output**
Paste in the http or JSON output

```json
{
  "newUsers": { "email": "tony@mantle-labs.com" }
}
```

OR

```http
    HTTP/1.1 200 OK
    date: Tue, 14 Jan 2025 11:07:53 GMT
    server: uvicorn
    content-length: 1063
    content-type: application/json
    Connection: close

    {
      "newUsers": {"email": "tony@mantle-labs.com"}
    }
```

**Additional context**
Add any other context about the problem here.
