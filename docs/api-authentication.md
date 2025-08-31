# Authentication

Some APIs require authentication (a way to prove who you are).  
JSONPlaceholder doesn’t need it, but here’s a simple example you might see in real APIs.

---

## API Key example
Some APIs give you a key like this:  

12345-ABCDE-SECRET


You include it in your request header:  
```bash
curl -s https://api.example.com/data \
  -H "Authorization: Bearer 12345-ABCDE-SECRET"


