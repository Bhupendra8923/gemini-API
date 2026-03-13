# 🧑‍🏫 Gemini AI Chat Panel

A lightweight, single-file HTML chatbot powered by **Google Gemini 2.5 Flash**.  
Features a strict father/teacher persona — and is **100% safe to push to GitHub** because your API key is never stored in the code.

---

## 🔒 How the API Key is Protected

| Method | This Project |
|--------|-------------|
| Hardcoded in code | ❌ Never |
| Saved in localStorage | ❌ Never |
| Pushed to GitHub | ❌ Never |
| Stored in session memory only | ✅ Yes |

Your API key is entered by **you** at runtime in the browser.  
It lives only in memory and disappears the moment you close or refresh the tab.  
**Bots scanning GitHub will find nothing.**

---

## ✨ Features

- 🔑 API key entered at runtime — never in the source code
- 🧑‍🏫 Strict father/teacher AI persona
- 💬 Clean modern chat UI with typing indicator
- 🌙 Dark mode design
- ⚡ Zero dependencies — single HTML file, no build tools needed
- 🔁 Change API key anytime without refreshing

---

## 🚀 Getting Started

### 1. Get a Free Gemini API Key

Go to 👉 [https://aistudio.google.com/app/apikey](https://aistudio.google.com/app/apikey)  
Click **"Create API Key"** and copy it.

### 2. Open the App

Just open `index.html` in your browser — no server needed.

```
Double-click index.html
```

Or run a local server:

```bash
# Python
python -m http.server 8080

# Node.js
npx serve .
```

Then open `http://localhost:8080`

### 3. Enter Your Key & Chat

- Paste your Gemini API key in the input box
- Click **"Start Chatting"**
- Your key stays in memory only — never saved anywhere

---

## 📁 Project Structure

```
index.html    ← Entire app (HTML + CSS + JS in one file)
README.md     ← This file
```

No `.env` file, no config file, no backend — just one HTML file.

---

## ⚙️ Customization

### Change the AI Persona

Open `index.html` and find this line:

```javascript
const persona =
  "You are a strict father and a teacher by profession. " +
  "You follow discipline and rules. Answer seriously like a father teaching his child. " +
  "Do not introduce yourself. The message is: ";
```

Edit the text to give the AI any personality you want.

### Change the Model

Find this line in the `fetch()` call:

```javascript
`https://generativelanguage.googleapis.com/v1beta/models/gemini-2.5-flash:generateContent?key=${API_KEY}`
```

Replace `gemini-2.5-flash` with any supported Gemini model name.

---

## ✅ Safe to Push to GitHub Checklist

- ✅ No API key in the source code
- ✅ No API key in localStorage
- ✅ No `.env` file needed
- ✅ README explains how to get and use an API key
- ✅ Users enter their own key at runtime

**You can push this project to a public GitHub repo without any risk.**

---

## ⚠️ Limitations

- No conversation memory — each message is sent independently
- Requires an active internet connection
- API key must be re-entered after each page refresh (by design, for security)

---

## 📄 License

Free to use for personal and educational purposes.
