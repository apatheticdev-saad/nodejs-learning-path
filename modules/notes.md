# 📦 Node.js Modules

## 🔹 What are Modules?

Modules are reusable pieces of code that help organize applications.

---

## 🔹 Types of Modules

### 1. Core Modules

Built-in modules (no installation needed)
Examples: `fs`, `http`, `path`

```js
const fs = require('fs');
```

---

### 2. Local Modules

Custom files created by developer

```js
// math.js
function add(a, b) {
  return a + b;
}
module.exports = { add };

// app.js
const math = require('./math');
console.log(math.add(2, 3));
```

---

### 3. Third-party Modules

Installed using npm

```bash
npm install express
```

---

## 🔹 Using Express (Example)

```js
const express = require('express');
const app = express();

app.get('/', (req, res) => {
  res.send('Hello World');
});

app.listen(3000);
```

---

## 🔹 CommonJS vs ES Modules

### CommonJS

* `require()`
* `module.exports`

### ES Modules

* `import` / `export`
* Modern approach  

---

## 🔹 Summary

* Modules make code reusable & organized
* Types: Core, Local, Third-party
* Essential concept in Node.js development⚡
