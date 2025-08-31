# Error Handling

APIs return status codes and messages. Use this page to understand common errors and what to do next.

---

## Quick reference

| Status | Meaning           | What you should do                         |
|------:|--------------------|--------------------------------------------|
| 200   | OK                 | All good                                   |
| 201   | Created            | Resource created                           |
| 400   | Bad Request        | Fix your JSON or query parameters          |
| 401   | Unauthorized       | Add/refresh your API key or token          |
| 403   | Forbidden          | You don’t have permission                  |
| 404   | Not Found          | Check the URL or resource ID               |
| 429   | Too Many Requests  | Slow down; add retry/backoff               |
| 500   | Server Error       | Try again later; capture request details   |

---

## Example: 404 Not Found
Requesting a user that doesn’t exist:
```bash
curl -i https://jsonplaceholder.typicode.com/users/9999
HTTP/1.1 404 Not Found
curl -s https://jsonplaceholder.typicode.com/users | head
curl -s -X POST https://jsonplaceholder.typicode.com/posts \
  -H "Content-Type: application/json" \
  -d '{ "title": 123 }'    # title should be a string
curl -s -X POST https://jsonplaceholder.typicode.com/posts \
  -H "Content-Type: application/json" \
  -d '{ "title": "Hello", "body": "First post", "userId": 1 }'

Reply “done” when saved, and I’ll give you the **one-line change** to add it to your menu.

