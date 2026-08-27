# 🌟 Vibecode Editor - Next-Gen Web Development Environment

![Vibecode Editor Preview](public/vibe-code-editor-thumbnaail.svg)

**Vibecode Editor** revolutionizes web development by combining the power of a full-featured IDE with AI assistance, all running directly in your browser. Built on cutting-edge technologies like Next.js 15, WebContainers, and local AI models, it provides a seamless development experience without the need for local environment setup.

## ✨ Why Choose Vibecode Editor?

- 🚀 **Zero-Config Development** - Start coding instantly with pre-configured project templates
- 🤖 **AI-First Development** - Get intelligent code suggestions powered by local LLMs (via Ollama)
- 💻 **Full-Stack in Browser** - Run both frontend and backend code directly in your browser
- 🔒 **Privacy Focused** - Keep your code private with local AI processing
- 🌈 **Beautiful & Productive** - Modern UI with dark/light themes and keyboard shortcuts

## 🛠 Core Features

### 🧩 Smart Code Editor
- Monaco Editor (same as VS Code) with syntax highlighting
- AI-powered autocompletion and code suggestions
- Multiple cursor support and advanced editing features

### ⚡ Real-Time Execution
- Run React, Node.js, and more directly in the browser
- Built-in terminal with xterm.js
- Instant preview of your application

### 🔄 Seamless Integration
- GitHub and Google authentication
- Import/export projects with ease
- Extensible architecture for adding new features

### 🤖 AI-Powered Assistance
- Context-aware code completion
- AI chat assistant for code explanations
- Refactoring suggestions and bug detection

## 🧱 Tech Stack

| Layer         | Technology                                   |
|---------------|----------------------------------------------|
| Framework     | Next.js 15 (App Router)                      |
| Styling       | TailwindCSS, ShadCN UI                       |
| Language      | TypeScript                                   |
| Auth          | NextAuth (Google + GitHub OAuth)             |
| Editor        | Monaco Editor                                |
| AI Suggestion | Ollama (LLMs running locally via Docker)     |
| Runtime       | WebContainers                                |
| Terminal      | xterm.js                                     |
| Database      | MongoDB (via DATABASE_URL)                   |

---

## 🛠️ Getting Started

### 1. Clone the Repo

```bash
git clone https://github.com/your-username/vibecode-editor.git
cd vibecode-editor
````

### 2. Install Dependencies

```bash
npm install
```

### 3. Set Up Environment Variables

Create a `.env.local` file using the template:

```bash
cp .env.example .env.local
```

Then, fill in your credentials:

```env
AUTH_SECRET=your_auth_secret
AUTH_GOOGLE_ID=your_google_client_id
AUTH_GOOGLE_SECRET=your_google_secret
AUTH_GITHUB_ID=your_github_client_id
AUTH_GITHUB_SECRET=your_github_secret
DATABASE_URL=your_mongodb_connection_string
NEXTAUTH_URL=http://localhost:3000
```

### 4. Start Local Ollama Model

Make sure [Ollama](https://ollama.com/) and Docker are installed, then run:

```bash
ollama run codellama
```

Or use your preferred model that supports code generation.

### 5. Run the Development Server

```bash
npm run dev
```

Visit `http://localhost:3000` in your browser.


---

## 🎯 Keyboard Shortcuts

* `Ctrl + Space` or `Double Enter`: Trigger AI suggestions
* `Tab`: Accept AI suggestion
* `/`: Open Command Palette (if implemented)

---



---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 🙏 Acknowledgements

* [Monaco Editor](https://microsoft.github.io/monaco-editor/)
* [Ollama](https://ollama.com/) – for offline LLMs
* [WebContainers](https://webcontainers.io/)
* [xterm.js](https://xtermjs.org/)
* [NextAuth.js](https://next-auth.js.org/)

```
