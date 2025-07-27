# AI-Chatbot

A modern, full-stack AI chatbot application powered by Google Gemini API. Features a clean, responsive chat UI built with Next.js and Tailwind CSS, and a Node.js/Express backend that securely proxies requests to Gemini.

---

## Features
- Conversational AI chatbot interface
- Google Gemini API integration (backend proxy)
- Modern, responsive UI (Next.js, Tailwind CSS)
- Reusable UI components
- Error handling and loading states
- Easy local development and deployment

---

## Tech Stack
- **Frontend:** Next.js, React, Tailwind CSS, TypeScript
- **Backend:** Node.js, Express, Axios, dotenv, CORS
- **AI:** Google Gemini API

---

## Getting Started

### 1. Clone the Repository
```sh
git clone <your-repo-url>
cd AI-Chatbot
```

### 2. Setup the Backend (Server)
```sh
cd server
npm install
```

#### Configure Environment Variables
Create a `.env` file in the `server/` directory:
```
GEMINI_API_KEY=your_google_gemini_api_key_here
```

> **Note:** You must enable billing and the Gemini API in your Google Cloud project to use the API. See [Gemini API docs](https://ai.google.dev/gemini-api/docs/quickstart).

#### Start the Server
```sh
npm start
```
- The server runs on `http://localhost:5000` by default.

---

### 3. Setup the Frontend (Client)
```sh
cd ../client
npm install
```

#### Start the Client
```sh
npm run dev
```
- The client runs on `http://localhost:3000` by default.

---

## Usage
- Open [http://localhost:3000](http://localhost:3000) in your browser.
- Type a message and click **Send**. The message is sent to the backend, which calls the Gemini API and returns the AI's response.

---

## Project Structure
```
AI-Chatbot/
  client/    # Next.js frontend
  server/    # Express backend (Gemini proxy)
```

---

## Troubleshooting
- **429/Quota errors:** You may need to add a payment method and enable billing in Google Cloud to use the Gemini API.
- **CORS errors:** Ensure the backend is running and accessible at `http://localhost:5000`.
- **API key errors:** Double-check your `.env` file and that the Gemini API is enabled for your project.

---

## License
[MIT](LICENSE)
