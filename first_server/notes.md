# 🌐 Creating First Node.js Server

## 🔹 Steps to Create a Basic Server

### 1. Initialize Project

```bash
npm init -y
```

### 2. Create File

Create `app.js`

---

## 🔹 Basic HTTP Server Code

```js
const http = require('http');

const server = http.createServer((req, res) => {
  res.statusCode = 200;
  res.setHeader('Content-Type', 'text/plain');
  res.end('Hello, World!');
});

const port = 3000;

server.listen(port, () => {
  console.log(`Server running at http://localhost:${port}`);
});
```

---

## 🔹 Run Server

```bash
node app.js
```

👉 Open browser → `http://localhost:3000`

---

## 🔹 What is Happening?

* `http` → Core module
* `createServer()` → Creates server
* `req` → Request object
* `res` → Response object
* `listen()` → Starts server

---

## 🔹 Summary

* Created a simple server using Node.js
* Learned how server responds to requests
* Understood basic backend flow 🚀
