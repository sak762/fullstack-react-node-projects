# Real Chat App

This project is a simple real-time chat application with separate `frontend` and `backend` folders.

- `backend/` contains the Node.js + Express + Socket.IO server.
- `frontend/` contains the React chat UI.

## Prerequisites

- Node.js installed (recommended v18+)
- npm available in your terminal

## Backend

The backend runs a WebSocket server using Socket.IO.

### Start backend

1. Open a terminal in `backend/`
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the server:
   ```bash
   node server.js
   ```

The server listens on `http://localhost:4600`.

### What it does

- Accepts incoming socket connections
- Joins users to a shared room (`group`)
- Broadcasts events to other users:
  - `roomNotice`
  - `chatMessage`
  - `typing`
  - `stopTyping`

## Frontend

The frontend is a React app built with Create React App.
It connects to the backend at `http://localhost:4600`.

### Start frontend

1. Open a terminal in `frontend/`
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the React app:
   ```bash
   npm start
   ```

The app runs at `http://localhost:3000` by default.

## Usage

1. Start the backend server first.
2. Start the frontend.
3. Open the frontend URL in your browser.
4. Enter your name to join the chat.
5. Type messages and send them.

## Notes

- The frontend uses `socket.io-client` to connect to the backend.
- The backend uses `socket.io` to manage real-time events.
- Typing notifications are sent while the user is typing and stop after 1 second of inactivity.

## Folder structure

- `backend/server.js` — backend server logic
- `frontend/src/App.js` — main chat UI and state handling
- `frontend/src/ws.js` — socket connection helper
