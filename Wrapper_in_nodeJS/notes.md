# 🧩 Node.js Wrapper Function

## 🔹 What is Wrapper Function?

Every Node.js file is wrapped inside a function internally:

```js
(function(exports, require, module, __filename, __dirname) {
  // Your code
});
```

👉 This gives each file its own **private scope**

---

## 🔹 Special Variables

### 📄 __filename

Returns full path of current file

```js
console.log(__filename);
```

---

### 📁 __dirname

Returns directory path

```js
console.log(__dirname);
```

---

### 📦 module & exports

Used to export data/functions

---

### 📥 require()

Used to import modules

---

## 🔹 Why It Matters

* Prevents global scope pollution
* Provides module system
* Keeps code isolated

---

## 🔹 Example

```js
console.log('File:', __filename);
console.log('Directory:', __dirname);
```

---

## 🔹 Summary

* Node wraps every file inside a function
* Provides useful variables
* Helps manage modular architecture 🚀
