# EduManage (Client)

## Overview

A MERN-based education management platform with role-based dashboards for students, teachers, and admins—covering classes, enrollments with payments, assignments, approvals, and comprehensive admin controls.  
This repository contains the client-side React application.

Live Preview:  
https://edu-manage-ed474.web.app/

---

## Table of Contents

- [Project Description](#project-description)
- [Features](#features)
- [Technology Used](#technology-used)
- [Installation](#installation)
- [Usage](#usage)
- [Configuration](#configuration)
- [Contributing](#contributing)
- [Testing](#testing)
- [License](#license)
- [Contact / Support](#contact--support)

---

## Project Description

EduManage (Client) is an advanced, responsive ReactJS web application for education management. It connects students, teachers, and admins in a seamless, interactive environment to manage classes, assignments, enrollment, and platform-wide administration with a focus on usability, security, and performance.  
The client interacts with a separate backend API for data persistence, authentication, and payments.

---

## Features

- **Modern Responsive Design:** Fully responsive layout using CSS Grid and Flexbox.
- **Routing:** Client-side navigation with React Router.
- **Role-Based Dashboards:** Dedicated dashboards for students, teachers, and admins with tailored functionality.
- **Secure Authentication:** Email/password and Google authentication with JWT-based protected routes.
- **Class Management:** Teachers can add, update, and delete classes, pending admin approval before listing.
- **Class Enrollment & Payment:** Students can enroll and pay for classes; enrollment and transactions are tracked.
- **Assignment Workflow:** Teachers create assignments; students submit and track progress in real time.
- **Teaching Application:** Users can apply to become teachers; admins review and approve.
- **Admin Control:** Admins approve/reject teacher applications and classes, manage users, and oversee platform data.
- **Pagination and Search:** Paginated tables/cards and server-side search for efficient data handling.
- **Accessibility:** Focus states and screen reader-friendly markup.
- **Smooth Animations:** Subtle transitions for interactive elements.
- **Security Best Practices:** Sensitive keys (Firebase, etc.) are secured with environment variables.

---

## Technology Used

- **React** — Frontend library for building user interfaces
- **React Router DOM** — Declarative routing for React applications
- **Firebase Authentication** — Email/Password and Google sign-in
- **JSON Web Tokens (JWT)** — Client-side handling for protected routes
- **React Hook Form** — Form handling and validation
- **Axios/Fetch** — HTTP requests to the backend API
- **CSS3** — Styling and layout using Grid and Flexbox

---

## Installation

### Prerequisites

- [Git](https://git-scm.com/) (to clone the repository)
- [Node.js](https://nodejs.org/) and [npm](https://www.npmjs.com/) (for dependency management)
- A modern web browser (Chrome, Edge, Firefox, Safari, etc.)

### Steps

1. **Clone the repository:**
   ```bash
   git clone https://github.com/usernayeem/edu-manage.git
   ```

2. **Navigate to the project directory:**
   ```bash
   cd edu-manage
   ```

3. **Install dependencies:**
   ```bash
   npm install
   ```
4. Create and configure environment variables (see Configuration).

5. **Run locally:**
   ```bash
   npm run dev
   ```
   This will start the development server. The app will be available at `http://localhost:5173`.

---

## Usage

- **Sign In / Sign Up:** Authenticate via Email/Password or Google to access role-based dashboards.
- **Students:** Browse approved classes, enroll and pay, view enrolled classes, and submit assignments.
- **Teachers:** Apply to become a teacher, create and manage classes, post assignments, and review submissions.
- **Admins:** Review and approve teacher applications and classes, manage users/roles, and monitor platform activity.
- **Pagination & Search:** Use built-in pagination and search to navigate large datasets efficiently.

- **Admin Demo Credentials:**
  - Email/Password:
    - Email: `nayeem.edumanage@mailinator.com`
    - Password: `qwerty123`
  - Google:
    - Email: `nayeem.edumanage@gmail.com`
    - Password: `qwertynayeem`

---

## Configuration

- Environment variables (create a `.env` file in the project root):
  ```env
  VITE_API_BASE_URL=http://localhost:5173
  VITE_FIREBASE_API_KEY=your_firebase_api_key
  VITE_FIREBASE_AUTH_DOMAIN=your_firebase_auth_domain
  VITE_FIREBASE_PROJECT_ID=your_firebase_project_id
  VITE_FIREBASE_STORAGE_BUCKET=your_firebase_storage_bucket
  VITE_FIREBASE_MESSAGING_SENDER_ID=your_firebase_messaging_sender_id
  VITE_FIREBASE_APP_ID=your_firebase_app_id
  ```

- Styling: Modify the main stylesheet (e.g., `index.css`) or your chosen UI utility/classes to customize design.

---

## Contributing

Contributions are welcome! If you would like to contribute to this project, follow these steps:

1. **Fork the Repository**:

   - Navigate to the repository you want to contribute to.
   - Click the **Fork** button in the upper right corner to create a personal copy of the project in your GitHub account.

2. **Clone the Forked Repository**:

   - Open your forked repository on GitHub.
   - Click the "Code" button to get the HTTPS or SSH URL of your forked repository.
   - Open your terminal or command prompt.
   - Use the `git clone` command followed by the URL you copied to clone the repository to your local machine:

     ```bash
     git clone https://github.com/yourusername/edu-manage.git
     ```

     Replace `yourusername` with your own Github username.

   - Navigate into the cloned repository directory:
     ```bash
     cd edu-manage
     ```

3. **Create a New Branch**: Switch to a new branch where you'll make your changes. You can do this using the following command:

   ```bash
   git checkout -b my-branch
   ```

   Replace `my-branch` with a branch name that describes your work.

4. **Make Your Changes**: Make the necessary changes to the codebase. You can add, modify, or delete files as needed.

5. **Stage Your Changes**: You can use `git add <filename>` to stage specific files or `git add .` to stage all changes.

   ```bash
   git add .
   ```

6. Commit Your Changes: Commit your staged changes with a descriptive message. Follow the imperative style for commit messages (e.g., “Fix bug” instead of “Fixed bug”). For example:

   ```bash
   git commit -m "my commit message"
   ```

   Replace `my commit message` with a meaningful message for your commit.

7. **Push to Your Branch**: Push your changes to the branch you created:

   ```bash
   git push -u origin my-branch
   ```

   Replace `my-branch` with your branch name.

8. **Submit a Pull Request**:
   - Navigate to your forked repository on GitHub.
   - Click the "Compare & pull request" button.
   - Review the changes you're proposing and ensure they are accurate.
   - Add a descriptive title and a detailed description of your contribution.
   - Click the "Create pull request" button to submit your contribution for review.

---

## Testing

- **Automated Testing:**  
  The project can use Jest and React Testing Library for unit and component testing (if configured).

- **Run Tests:**
  ```bash
  npm test
  ```

- **For manual testing:**
  - Open the app in different browsers and devices.
  - Test keyboard navigation and accessibility.
  - Check responsiveness on various screen sizes.
  - Verify protected routes and role-based access control (student/teacher/admin).
  - Exercise CRUD flows (classes, assignments, enrollments) and confirm notifications.

---

## License

This project is licensed under the [MIT](LICENSE) License.

---

## Contact / Support

- **Author:** [Md Nayeem](https://www.github.com/usernayeem)
- **Repository**: https://github.com/usernayeem/edu-manage
- **Issues:** Please use the [GitHub Issues page](https://github.com/usernayeem/edu-manage/issues) for bug reports or feature requests.
