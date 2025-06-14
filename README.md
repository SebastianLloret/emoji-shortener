# Emoji URL Shortener 🔗😄

A playful and functional URL shortener that uses emoji as short codes. Built as a take-home assignment to demonstrate backend fundamentals, this project turns long URLs into fun, emoji-based short links.

## 🚀 Features

- Shorten URLs using emojis as identifiers.
- Basic in-memory storage (no external database required).
- Express.js server with minimal dependencies.
- Fully functional API to create and resolve emoji-shortened links.

## 🛠️ Tech Stack

- **Node.js**
- **Express.js**

## 📦 Installation

```bash
git clone git@github.com:SebastianLloret/emoji-shortener.git
cd emoji-shortener
npm install
```

## ▶️ Running the Server

```bash
node app.js
```

The server will start on `http://localhost:3000`.

## 📌 Usage

### Shorten a URL

Send a `POST` request to `/shorten` with JSON:

```json
{
  "url": "https://example.com"
}
```

**Response:**

```json
{
  "short": "😄"
}
```

### Visit the Shortened URL

Access `http://localhost:3000/😄` to be redirected to the original URL.

## ⚠️ Notes

- This is a simple, stateless demo using in-memory storage. Restarting the server will reset all data.
- Emoji handling depends on URL encoding in the client/browser.
