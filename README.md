
# Personal Voice Bot

A modern, animated web-based voice bot UI that lets users interact with an AI agent using text or voice. Built with HTML, CSS, and JavaScript, and connects to an n8n AI agent for responses.

## ✨ Features

- **Voice Input:** Start and stop voice recording using your browser's speech recognition.
- **Text Input:** Type questions and get instant replies.
- **Predefined Questions:** Click on suggested questions to quickly interact.
- **Animated UI:** Smooth fade-in, floating bot icon, and interactive chat bubbles.
- **Text-to-Speech:** Bot replies are spoken aloud.
- **Responsive Design:** Works well on desktop and mobile.

## 🚀 Getting Started

### 1. Clone the repository

```sh
git clone https://github.com/UppalRahi/HomeLLC.git
cd HomeLLC
```

### 2. Run Locally

You need to serve the files using a local web server for full functionality (especially for microphone access).

**With Python 3:**
```sh
python3 -m http.server 8000
```
Open [http://localhost:8000/index.html](http://localhost:8000/index.html) in your browser.

**With Node.js (if installed):**
```sh
npx serve .
```

### 3. Usage

- Click **Start Recording** to ask a question by voice.
- Type your question and click **Send** to chat by text.
- Click any predefined question chip to send it instantly.
- The bot will reply in text and voice.

## 🛠️ Configuration

- The bot sends user questions to an n8n webhook.  
- To use your own n8n agent, update the `WEBHOOK_URL` in `index.html`:

```js
const WEBHOOK_URL = "https://your-n8n-instance/webhook/your-webhook-id";
```

## 📱 Browser Support

- Works best in Chrome and Edge (for voice recognition).
- Speech recognition may not be supported in Firefox or Safari.

## 📦 Deployment

You can host this on [GitHub Pages](https://pages.github.com/), [Vercel](https://vercel.com/), [Netlify](https://netlify.com/), or any static web host.

## 🙏 Credits

- UI/UX: [UppalRahi](https://github.com/UppalRahi)
- Backend: [n8n](https://n8n.io/)

---

**Enjoy chatting with your Personal Voice
