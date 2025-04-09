# Todo List Portfolio Website

A user-authenticated To-Do List web application built with Flask, Bootstrap 5, and SQLAlchemy. Users can register, log in, and manage their personal task lists. This project is designed to demonstrate full-stack web development skills using Python and Flask.

---

## Features

- User registration and login system with secure password hashing
- Session-based user authentication using Flask-Login
- Add and view to-do items, unique to each user
- Flash messages for feedback (e.g., duplicate email, login errors, success)
- Responsive UI with Bootstrap 5 and CKEditor integration
- Clean folder and template structure for scalability

---

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/ulquiorraexe/todo-list-portfolio-website.git
2. Navigate to the project directory:
   ```bash
   cd todo-list-portfolio-website
3. Install the required packages:
   ```bash
   pip install -r requirements.txt
4. (Optional) Set environment variables for security:
   ```bash
   export FLASK_SECRET_KEY="your-secret-key"
   export DB_URI="sqlite:///posts.db"
5. Run the application:
   ```bash
   python main.py
6. Open your browser and go to:
   ```arduino
   http://localhost:5500

## Usage Examples

### Register a New User

1. Go to `/register`
2. Fill out the registration form
3. Submit to create an account and get logged in automatically

### Log In

1. Navigate to `/login`
2. Enter your email and password
3. Gain access to your to-do lists

### Create a To-do

1. Go to `/create`
2. Enter your list content in the rich text editor (CKEditor)
3. Submit to save your to-do

### View Your To-dos

- Visit `/lists` to see all your saved to-do items
- Each list shows its content and creation date

### Persistence

- User and to-do data are saved in `posts.db` using SQLAlchemy ORM
- Relationships are set between users and their respective to-do items

### Log Out

- Go to `/logout` to securely log out of your account

## Project Structure
```text
.
├── main.py
├── forms.py
├── templates/
│   ├── header.html
│   ├── footer.html
│   ├── login.html
│   ├── register.html
│   ├── my_lists.html
│   ├── create_list.html
│   └── ...
├── static/
│   └── assets/
├── requirements.txt
└── README.md
```

## License

This project does not have a license.
