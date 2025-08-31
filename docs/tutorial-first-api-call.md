# Tutorial: Make Your First API Call in 5 Minutes

This tutorial walks you through calling the JSONPlaceholder API.  
By the end, you’ll have made your first real API request.

---

## Prerequisites
- A computer with **curl** installed (Mac and Linux have it by default).  
- Internet connection.

---

## Step 1 — Open your terminal
On Mac: **Applications → Utilities → Terminal**.  
You’ll see a prompt like this:  
juelmahoney@Juels-Air ~ %


---

## Step 2 — Try a simple request
Run this command:
```bash
curl -s https://jsonplaceholder.typicode.com/posts/1

Expected response (shortened):

{
  "userId": 1,
  "id": 1,
  "title": "sunt aut facere repellat provident occaecati",
  "body": "quia et suscipit..."
}

---


## Step 3 — Create your own resource

Use POST to create a fake post:


curl -s -X POST https://jsonplaceholder.typicode.com/posts \
  -H "Content-Type: application/json" \
  -d '{"title":"My First Post","body":"Hello world!","userId":1}'

Expected response: 


  "title": "My First Post",
  "body": "Hello world!",
  "userId": 1,
  "id": 101

---

## Step 4 — Explore further

Now that you can send GET and POST requests, try experimenting:

- Change the `title` or `body` values in your POST request.  
- Explore different endpoints like `/users` or `/comments`.  
- Try combining commands, for example:  

```bash
curl -s https://jsonplaceholder.typicode.com/users/1

Expected response (shortened):

{
  "id": 1,
  "name": "Leanne Graham",
  "email": "Sincere@april.biz"
}

