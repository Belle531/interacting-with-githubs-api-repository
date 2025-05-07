
# GitHub API Interaction Using Postman

This document outlines how to interact with GitHub’s API using Postman, including retrieving user information and creating a new repository. It provides step-by-step instructions along with screenshots to demonstrate the API requests.

## Retrieving User Info
To fetch information about your GitHub repositories using Postman, follow these steps:

1. Open Postman and select the "GitHub API" environment.
2. Define a variable `baseUrl` set to `https://api.github.com/`.
3. Create a **GET request** with the following URL:

4. Under the **Authorization** tab:
- Select **Bearer Token**.
- Input your personal GitHub token.
5. Ensure **Headers** contain:

6. Click **Send** to execute the request.
7. If successful, you will receive a JSON response listing your repositories.
8. Below is an example response:
```json
[
  {
    "id": 123456789,
    "name": "sample-repo",
    "html_url": "https://github.com/yourusername/sample-repo"
  }
]
