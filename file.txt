RBAC Admin Dashboard

This is a Role-Based Access Control (RBAC) Admin Dashboard built with React. The app allows administrators to manage users, roles, and permissions. Users can be assigned roles with specific permissions, and administrators can manage the status of users (active or inactive).

Table of Contents

Features
Technologies Used
Installation
Usage
Directory Structure
API Mock
License
Features
User Management:

View, add, edit, and delete users.
Assign roles to users.
Manage user status (active/inactive).
Role Management:

Define new roles with custom permissions.
Edit existing roles.
Delete roles.
Permissions:

Roles can have permissions like "Read", "Write", and "Delete".
Permissions are dynamically assigned to roles.
Responsive UI:

A user-friendly and responsive interface using Material UI components.
Routing:

Users can navigate between pages for user and role management.
Technologies Used
React: The frontend library used to build the UI.
React Router: For routing between different pages (Users and Roles).
Material-UI: For UI components such as DataGrid, Modal, and TextFields.
Formik: For form handling and validation.
Yup: For input validation using schema-based validation.
Mock API: Simulates API calls for user and role CRUD operations.
Installation
Follow the steps below to run the project locally:

1. Clone the Repository
Clone the project repository to your local machine:

git clone https://github.com/your-username/rbac-dashboard.git
cd rbac-dashboard
2. Install Dependencies
Run the following command to install the required dependencies:

npm install
3. Start the Application
After installing the dependencies, start the React development server:

npm start
This will start the application on http://localhost:3000.

Usage
Once the app is running, you can:

Manage Users:
Add new users by clicking on the Add User button.
View and delete users.
Assign roles like Admin or User to the users.
Manage Roles:
View existing roles.
Add new roles by clicking on the Add Role button.
Define the permissions for each role (e.g., Read, Write, Delete).
Delete roles as needed.
Directory Structure
Here's the file structure of the project:

rbac-dashboard/
├── public/
│   ├── index.html        # Main HTML template
├── src/
│   ├── App.tsx           # Main app component
│   ├── index.tsx         # React entry point
│   ├── components/
│   │   ├── AddUserModal.tsx   # Modal for adding a user
│   │   ├── AddRoleModal.tsx   # Modal for adding a role
│   │   ├── UserTable.tsx      # User DataGrid table component
│   │   ├── RoleTable.tsx      # Role DataGrid table component
│   ├── api/
│   │   ├── mockApi.ts         # Mock API for user and role management
├── package.json            # Project dependencies
├── README.md               # This README file
├── tsconfig.json           # TypeScript configuration file
Main Files and Their Purpose:
App.tsx: The main React component that handles routing and includes the UI for managing users and roles.
components/: Contains UI components like UserTable, RoleTable, and modals (AddUserModal and AddRoleModal).
api/mockApi.ts: A mock API to simulate user and role data for CRUD operations.
index.tsx: The entry point for the React app.
API Mock
The application uses a mock API to simulate CRUD operations on users and roles. It’s not connected to a real backend but mimics the functionality of adding, deleting, and fetching data.

API Functions:
getUsers(): Fetches the list of users.
addUser(data): Adds a new user.
deleteUser(id): Deletes a user by ID.
getRoles(): Fetches the list of roles.
addRole(data): Adds a new role.
deleteRole(id): Deletes a role by ID.
These functions are simulated to return promises and provide data updates in the UI.















