# Collaborative Task Management System

The Collaborative Task Management System is a web-based application built using the MERN stack. This platform enables multiple users to collaborate on projects by creating, assigning, and managing tasks effectively. It provides features like user authentication, project management, task management, and advanced search and filtering.

## Project Links
- **Live Application:** [Task Management App](https://task-management-app-chi-swart.vercel.app/)
- **GitHub Repository:** [Task Management App Repo](https://github.com/ayadav44237/Task-Management-App)

## Features

1. **User Registration and Authentication**
   - User Registration: Users can register by providing their name, email, and password.
   - Authentication: Implemented using JSON Web Tokens (JWT) to ensure secure access.
   - Authorization: Only authenticated users can access the platform.

2. **Project Management**
   - Create, edit, and delete projects.
   - Projects include the following details:
     - Title
     - Description
     - Creation Date
     - Project Owner

3. **Task Management**
   - Add, edit, delete, and assign tasks within projects.
   - Tasks include the following details:
     - Title
     - Description
     - Status (To-Do, In Progress, Completed)
     - Drag and Drop
     - Assigned User
   - Tasks are displayed grouped by status (To-Do, In Progress, Completed).

4. **User Dashboard**
   - Displays all projects and tasks assigned to the user.
   - Provides a task summary (e.g., total tasks, completed tasks).

5. **Search and Filters**
   - Search functionality to find tasks by title or description.
   - Filters to sort tasks by status, Most Recent, and Oldest First.

## Technical Stack

### Frontend
- **React.js**
  - Functional components and hooks for dynamic UI.
  - React Router for navigation.
  - Form validation for user inputs.
  - Responsive design for usability across devices.

### Backend
- **Node.js** and **Express.js**
  - RESTful API for managing users, projects, and tasks.
  - Secure API handling with JWT-based authentication.

### Database
- **MongoDB**
  - Stores user information, project details, and tasks.
  - Relationships maintained between users, projects, and tasks.

## Installation and Setup

### Prerequisites
- Node.js (v14 or later)
- MongoDB
- npm or yarn

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/ayadav44237/Task-Management-App

2. Install dependencies
    ```javascript
    # For front-end
    cd frontend
    npm install
    
    # For back-end
    cd ../backend
    npm install
    ```
3. Set up environment variables
   - Create a `.env` file in the root directory of the server and add the following variables:
    ```javascript
    MONGO_URI = <your_mongo_db_uri>
    JWT_SECRET = <your_jwt_secret>
    GOOGLE_CLIENT_ID = <your_google_client_id>
    GOOGLE_CLIENT_SECRET = <your_google_client_secret>
    ```
4. Run the application
    ```javascript
    # Start the back-end server
    cd backend
    npm start
    
    # Start the front-end application
    cd ../frontend
    npm start
    ```
## Usage
1. Sign up or log in to your account.
2. Create a new task by clicking the "Add Task" button.
3. Drag and drop tasks between columns to organize them.
4. Update or delete tasks by clicking on the task and using the provided options.

## API Endpoints
1. User Routes
   - `POST /api/users/register`: Register a new user
   - `POST /api/users/login`: Log in a user
   - `POST /api/users/google-login`: Log in a user via Google
2. Task Routes
   - `GET /api/tasks`: Get all tasks
   - `POST /api/tasks`:  Create a new task
   - `PUT /api/tasks/:id`: Update a task
   - `DELETE /api/tasks/:id`: Delete a task

## Security
- Use environment variables for sensitive data.
- Implement JWT for authentication and secure API routes.
- Validate user inputs on both client and server sides.
- Use HTTPS in production.

## Contact
- For any questions or feedback, please contact:
  Email: ayadav44237@gmail.com



