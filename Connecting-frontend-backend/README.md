<<<<<<< HEAD
# Connecting Frontend and Backend

A full-stack web application with a Node.js/Express backend and a React frontend, connected together to fetch and display user data.

## Project Structure

```
.
├── backend/              # Express.js server
│   ├── index.js         # Main server file
│   ├── user.js          # User data
│   └── package.json
└── frontend/            # React application
    └── user-app/        # Create React App
        ├── public/
        ├── src/
        ├── package.json
        └── README.md
```

## Features

- **Backend:** RESTful API endpoints to serve user data
- **Frontend:** React app to fetch and display users from the backend
- **Data:** 11 sample users with detailed profiles (address, company, contact info)

## Getting Started

### Prerequisites

- Node.js (v14+)
- npm or yarn

### Backend Setup

1. Navigate to the `backend` folder:
   ```bash
   cd backend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the server:
   ```bash
   node index.js
   ```
   Server runs on `http://localhost:3000`

### Frontend Setup

1. Navigate to the `frontend/user-app` folder:
   ```bash
   cd frontend/user-app
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the React development server:
   ```bash
   npm start
   ```
   App opens on `http://localhost:3000` (or another port if 3000 is busy)

## API Endpoints

### Backend Routes

| Method | Endpoint      | Description           |
|--------|---------------|-----------------------|
| GET    | `/`           | Server status check   |
| GET    | `/api/users`  | Get all users         |

**Example Response:** `/api/users` returns a JSON array of user objects with id, name, email, address, phone, website, and company info.

## Running Both Servers

### In Separate Terminals

**Terminal 1 (Backend):**
```bash
cd backend
npm install
node index.js
```

**Terminal 2 (Frontend):**
```bash
cd frontend/user-app
npm install
npm start
```

The React app will automatically fetch data from the backend API at `http://localhost:3000/api/users`.

## Environment Variables

### Backend
- `PORT` — Server port (default: 3000)

## Technologies Used

- **Backend:** Node.js, Express.js
- **Frontend:** React, JavaScript
- **Data Format:** JSON

## License

MIT
=======
# fullstack-react-node-projects
Full-stack React and Node.js projects showcasing frontend development, REST APIs, AWS Lambda, DynamoDB, and modern JavaScript practices.
>>>>>>> cdbdbc7f907783b95651c64fc9aa883d8b3bf53e
