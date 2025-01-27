Authentication System
Project Overview
The Authentication System is a web-based application developed using Django for managing user authentication. It allows users to securely register, log in, and manage their profiles. The system uses Django's built-in authentication views along with JWT (JSON Web Tokens) for handling secure user sessions. The app supports user registration, login, password reset, and profile management functionalities.

This project aims to provide a secure and efficient way of handling user authentication in web applications.

Features
User Registration: Allows users to create accounts with a unique username and password.
User Login: Provides secure login using username and password.
Password Reset: Allows users to reset their passwords if forgotten.
JWT Authentication: Uses JSON Web Tokens (JWT) for maintaining secure user sessions.
Profile Management: Users can view and update their profile information.
Admin Panel: Admins can manage users, view activity, and handle authentication-related tasks via Django’s admin panel.
Technologies Used
Django: Framework used for backend development.
JWT (JSON Web Tokens): For token-based authentication.
SQLite: Default database used for user data storage (can be swapped for other databases).
Django Rest Framework: For API views and handling token-based authentication.
Installation
Clone the repository:

bash
Copy
Edit
git clone https://github.com/yourusername/authentication-system.git
cd authentication-system
Create a virtual environment and activate it:

bash
Copy
Edit
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Apply migrations:

bash
Copy
Edit
python manage.py migrate
Create a superuser (for admin panel access):

bash
Copy
Edit
python manage.py createsuperuser
Run the server:

bash
Copy
Edit
python manage.py runserver
The application will be accessible at http://127.0.0.1:8000.

Usage
Visit the login page to sign in or register a new user.
After logging in, you’ll be issued a JWT token for secure session management.
Admins can access the Django admin panel at http://127.0.0.1:8000/admin to manage user authentication.
API Endpoints
POST /api/register/: Register a new user.
POST /api/login/: Log in and receive a JWT token.
POST /api/logout/: Log out the user (token invalidation).
POST /api/password-reset/: Request a password reset.
GET /api/user-profile/: Get the logged-in user’s profile information.
PUT /api/user-profile/: Update the logged-in user’s profile.
Contributing
Fork the repository.
Create a new branch (git checkout -b feature/your-feature).
Commit your changes (git commit -m 'Add new feature').
Push to your branch (git push origin feature/your-feature).
Create a new Pull Request.
License
This project is licensed under the MIT License - see the LICENSE file for details.

Feel free to modify or enhance the README based on additional features or specific configurations in your project!
Built and managed by Ruchita Ghate
# Auth
