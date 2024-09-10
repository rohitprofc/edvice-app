
# Edvice App

Edvice App is a full-stack web application consisting of a frontend built with Vite + React and a backend using Express.js. This project provides a comprehensive platform for mentoring, where users can connect with industry leaders for career guidance and development.

## Folder Structure

The project structure is as follows:

```
edvice-app/
├── .git/
├── backend/
│   ├── package-lock.json
│   └── package.json
├── frontend/
│   ├── public/
│   ├── src/
│   ├── package-lock.json
│   └── package.json
├── .gitignore
├── LICENSE
└── README.md
```

## Prerequisites

Ensure you have the following installed on your machine:

- Node.js (version 14.x or later)
- npm (Node Package Manager)

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/rohitprofc/edvice-app.git
cd edvice-app
```

### 2. Install dependencies

#### Frontend

Navigate to the `frontend` directory and install the dependencies:

```bash
cd frontend
npm install
```

#### Backend

Navigate to the `backend` directory and install the dependencies:

```bash
cd ../backend
npm install
```

## Running the Application

### 1. Start the Backend Server

Open a terminal and navigate to the `backend` directory. Run the following command to start the Express server:

```bash
cd backend
npm start
```

By default, the backend server will run on [http://localhost:5000](http://localhost:5000).

### 2. Start the Frontend Development Server

Open a new terminal and navigate to the `frontend` directory. Run the following command to start the Vite development server:

```bash
cd frontend
npm run dev
```

By default, the frontend server will run on [http://localhost:5173](http://localhost:5173).

<!-- ## Environment Variables

You may need to set up environment variables for both the frontend and backend. Create a `.env` file in each directory (`frontend` and `backend`) with the required configurations.

### Backend `.env` Example:

```plaintext
PORT=5000
MONGO_URI=mongodb://localhost:27017/edvice
JWT_SECRET=your_jwt_secret
```

### Frontend `.env` Example:

```plaintext
VITE_API_URL=http://localhost:5000
```

## Building for Production

To build the project for production, follow these steps:

### 1. Build the Frontend

Navigate to the `frontend` directory and run:

```bash
cd frontend
npm run build
```

The production-ready files will be generated in the `frontend/dist` folder.

### 2. Deploy the Backend

Ensure the backend is configured properly for a production environment, including any necessary environment variables and optimizations. -->

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature-name`).
3. Commit your changes (`git commit -m 'Add your feature'`).
4. Push to the branch (`git push origin feature/your-feature-name`).
5. Open a Pull Request.

## Branching Strategy

A good branching strategy is essential to keep the codebase clean and avoid conflicts. Here is a recommended branching strategy:

- **main branch**:
  - The main branch should always have a stable version of the code. This is the production-ready code and should only contain tested, stable, and reviewed code.

- **dev branch**:
  - The dev branch is the integration branch where all feature branches are merged after code reviews. It serves as the main development branch where the latest, stable, but not yet production-ready code exists.

- **Feature branches**:
  - Feature branches are used to develop new features, fix bugs, or make changes. Each branch is created from the dev branch and merged back into dev after completion and review.
  - **Naming convention**: `feature/{feature-name}` or `fix/{bug-name}`. For example, `feature/frontend-login-page` or `fix/backend-socket-error`.

- **Hotfix branches**:
  - If there is an urgent fix needed on the main branch (e.g., a critical bug in production), you can create a hotfix branch from main.
  - **Naming convention**: `hotfix/{issue-name}`.


## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.