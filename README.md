# Kanban Board with JWT Authentication

## Description
This is a full-stack Kanban board application enhanced with secure authentication using JSON Web Tokens (JWT). JWTs provide a compact, URL-safe mechanism for encoding authentication data and verifying user identities, making it an ideal solution for scalable, secure applications. In this project, a pre-built Kanban board has been upgraded to include:

- **Secure Login:** A dedicated login page with form inputs for username and password.
- **Token-Based Authentication:** On successful login, a JWT is generated and stored securely in the client's local storage for authenticating subsequent API requests.
- **Robust Security Flow:** Invalid credentials trigger error messages, and expired sessions automatically redirect users back to the login page.
- **Seamless UI/UX:** After login, users access a fully interactive Kanban board where tasks are organized into columns (e.g., To Do, In Progress, Done).
- **Deployment Ready:** The application is configured to be deployed on Render, with all necessary settings for environment variables and database connections.

This project was developed as a challenge to integrate JWT authentication into an existing Kanban board application, ensuring a secure and user-friendly experience.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Screenshot](#screenshot)
- [Deployment](#deployment)
- [Contribution](#contribution)
- [Tests](#tests)
- [License](#license)
- [Questions](#questions)

## Installation

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   cd your-repo-name

2. Download the Starter Code:
Make sure to download and unzip the starter code files provided, then initialize your own repository using these files.

3. Install Dependencies:
Install all required packages by running: npm install

4. Configure Environment Variables:
In the server directory, create a .env file and add:
DB_USERNAME=your_db_username
DB_PASSWORD=your_db_password
JWT_SECRET=your_secret_key

## Usage

Starting the Application:
Launch the application by running:
npm start
Or, if you use a development workflow with concurrently running server and client:
npm run dev

Access the Login Page:
Open your browser and navigate to http://localhost:3000 (or your configured port). The login page will prompt you for your username and password.

Authentication Flow:

    Valid Login: Enter valid credentials to generate a JWT, store it in local storage, and be redirected to the main Kanban board.

    Invalid Login: Incorrect credentials will trigger an error message.

    Session Management: Logging out clears the stored JWT and redirects to the login page. Additionally, after a period of inactivity, the session expires, and the user is prompted to log in again.

## Screenshot

Home:
![alt text](<assets/Screenshot 2025-04-08 150333.png>)

Login:
![alt text](<assets/Screenshot 2025-04-08 150525.png>)

Kanban:
![alt text](<assets/Screenshot 2025-04-08 150613.png>)

## Deployment

Deployed website: https://kanban-board-n23e.onrender.com

## Contribution

Contributions are welcome! If you’d like to improve or extend the project:

    Fork the repository.

    Create a feature branch and implement your changes.

    Submit a pull request with a detailed description of your modifications.

## Tests

To ensure the application works as expected:

API Testing:
    Use Insomnia to import the provided JSON request collection and test the authentication endpoints directly.

Functional Testing:

    Launch the application.

    Attempt logins with both valid and invalid credentials.

    Verify that the JWT is correctly stored on successful login and removed upon logout.

    Confirm that the Kanban board updates in response to authentication status.

## License

This project is licensed under the BSD license.

## Questions

If you have any questions or need further assistance, please contact:

Email: michael.mangieri@yahoo.com

GitHub: github.com/hazyplebian



