You're running `json-server` but it's giving you a lot of **JSON parsing errors** — that means your `db.json` file has **invalid JSON syntax** (missing colons, quotes, or braces).

Let me help you in **two ways**:

---

## ✅ Part 1: Fixed `db.json` Example

Here’s a clean, working example of `db.json` you can use:

```json
{
  "users": [
    {
      "id": 1,
      "firstName": "Muzamil",
      "lastName": "Fatima",
      "age": 22
    },
    {
      "id": 2,
      "firstName": "Ali",
      "lastName": "Raza",
      "age": 25
    }
  ]
}
```

### ✅ How to fix:

1. Open `db.json` in VS Code
2. Paste the code above
3. Save the file
4. Run again:

   ```bash
   npx json-server db.json
   ```

Now visit:

* `http://localhost:3000/users` ✅

---

## ✅ Part 2: Step-by-step `README.md` for Setting Up JSON Server

Here is your clean `README.md` file:

---

```markdown
# React Blog API Setup (Using JSON Server)

This guide will help you set up a fake REST API using `json-server` in your React project.

---

## 📁 Folder Structure

```

react-blog/
│
├── api/            ← API folder with db.json
│   └── db.json
│
└── src/            ← Your React frontend

````

---

## 🚀 Step-by-Step Setup

### 1. Open terminal inside `api` folder

```bash
cd F:\Skill Set\Web Devlopment\ReactJS\react-blog\api
````

---

### 2. Install json-server

```bash
npm install json-server
```

---

### 3. Create `db.json` file

Create a file named `db.json` inside the `api/` folder.

Paste this sample content:

```json
{
  "users": [
    {
      "id": 1,
      "firstName": "Muzamil",
      "lastName": "Fatima",
      "age": 22
    },
    {
      "id": 2,
      "firstName": "Ali",
      "lastName": "Raza",
      "age": 25
    }
  ]
}
```

✅ Make sure:

* All keys are in **double quotes** `"like this"`
* There are **no missing commas** or extra brackets

---

### 4. Start the server

```bash
npx json-server db.json
```

### ✅ You should see:

```
JSON Server started on http://localhost:3000

Endpoints:
http://localhost:3000/users
```

---

### 5. Test in browser

Go to:
[http://localhost:3000/users](http://localhost:3000/users)

You’ll see the list of users in JSON format.

---

## 💡 Notes

* `json-server` watches your file — any edits to `db.json` will auto-update the API.
* Press `CTRL+C` to stop the server.
* You can use other routes like `/posts`, `/comments`, etc.

---

## 📌 Extra Commands

| Command                                   | Description                     |
| ----------------------------------------- | ------------------------------- |
| `npm fund`                                | Show packages that need funding |
| `npx json-server db.json`                 | Start fake API                  |
| `json-server --watch db.json --port 4000` | Start API on custom port        |

---

## 🛠 Troubleshooting

❌ If you see JSON errors:

* Use [https://jsonlint.com](https://jsonlint.com) to validate your `db.json`
* Always use valid JSON format (no single quotes `'`, no trailing commas)

---