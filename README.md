# MERN Stack Admin Dashboard

A full-stack admin dashboard application built with the MERN stack (MongoDB, Express.js, React.js, Node.js).

## Features

- Admin User Login with JWT Authentication
- Agent Creation & Management
- CSV/Excel File Upload and Distribution
- Modern Material-UI Interface
- Responsive Design

## Prerequisites

- Node.js (v14 or higher)
- MongoDB (local installation or MongoDB Atlas account)
- npm or yarn package manager

## Setup Instructions

1. Clone the repository:
```bash
git clone <repository-url>
cd mern-admin-dashboard
```

2. Install Backend Dependencies:
```bash
cd backend
npm install
```

3. Create a `.env` file in the backend directory with the following content:
```
PORT=5000
MONGODB_URI=mongodb://localhost:27017/admin-dashboard
JWT_SECRET=your-secret-key-here
```

4. Install Frontend Dependencies:
```bash
cd ../frontend
npm install
```

5. Start the Backend Server:
```bash
cd ../backend
npm start
```

6. Start the Frontend Development Server:
```bash
cd ../frontend
npm start
```

The application will be available at:
- Frontend: http://localhost:3000
- Backend API: http://localhost:5000

## API Endpoints

### Authentication
- POST /api/auth/login - Admin login

### Agents
- POST /api/agents - Create new agent
- GET /api/agents - Get all agents
- GET /api/agents/:id - Get agent by ID

### Lists
- POST /api/lists/upload - Upload and distribute list
- GET /api/lists/distributed - Get distributed lists

## File Upload Requirements

The system accepts the following file formats:
- CSV (.csv)
- Excel (.xls, .xlsx)

The file should contain the following columns:
- FirstName (Text)
- Phone (Number)
- Notes (Text)

## Contributing

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a new Pull Request
