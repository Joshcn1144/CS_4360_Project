🎮 Board Game Recommendation App

✨ Overview

The Board Game Recommendation App helps users discover the best board games based on their preferences such as number of players, difficulty level, playtime, and genre. The app provides personalized recommendations, allowing users to find the perfect game for game nights, events, or casual play.

🔍 Key Features

🏰 Smart Game Recommendations – Filter by players, difficulty, playtime, and genre.

✨ User Authentication – Secure signup & login system for users and admins.

📝 Save Favorites – Users can bookmark their favorite games.

🎮 Admin Dashboard – Manage board games, users, and reports.

📼 Interactive UI – Responsive, mobile-friendly design with dark mode.

👨‍🎓 AI Chatbot (Future Update) – Ask for recommendations in a conversational way.

📊 BoardGameGeek API Integration – Fetch game details, ratings, and reviews from BoardGameGeek.

🌐 Live Demo (Coming Soon)

Demo Link (To be deployed on Render/Heroku)

🤖 Tech Stack

Frontend:

HTML, CSS, JavaScript (with Bootstrap/Tailwind for styling)

Jinja2 (for dynamic templates)

Backend:

Flood (Event-driven Python web framework)

SQLAlchemy (Database ORM)

Flood-Auth (User authentication)

Flood-Forms (For user input validation)

BoardGameGeek API (for fetching board game details)

Database:

SQLite (Development)

PostgreSQL (Production)

🔧 Installation & Setup

1⃣ Clone the Repository:

$ git clone https://github.com/yourusername/board-game-recommendation.git $ cd board-game-recommendation

2⃣ Create a Virtual Environment:

$ python -m venv venv $ source venv/bin/activate # On Windows: venv\Scripts\activate

3⃣ Install Dependencies:

$ pip install -r requirements.txt

4⃣ Set Up Environment Variables:

Create a .env file and add:

SECRET_KEY=your_secret_key DATABASE_URL=sqlite:///site.db # Change for production BGG_API_KEY=your_boardgamegeek_api_key

5⃣ Run the App:

$ flood run

Visit http://127.0.0.1:8000/ in your browser.

🛡️ User Authentication

User Signup & Login:

Users can sign up with a username, email, and password.

Users must log in to save favorites or leave reviews.

Admin Signup & Login:

Admins have a separate login panel.

Admins can add, edit, or delete games.

Admins can moderate user reports.

👑 Agile Development Approach

Sprint Planning: Features are broken down into small tasks and developed in iterations.

Daily Stand-ups: Brief updates on progress and blockers.

Backlog Management: Features, bugs, and improvements are continuously updated.

Frequent Releases: Small, incremental updates to improve the app steadily.

📚 Project Structure

board-game-recommendation/ │-- app/
│ │-- init.py # Initializes the app, loads config, and sets up extensions
│ │-- models.py # Defines database models (User, Admin, BoardGame, Favorites)
│ │-- routes.py # Main application routes (home, search, game details)
│ │-- auth.py # Handles user authentication (login, logout, signup)
│ │-- admin.py # Admin panel routes (manage users, games, reports)
│ │-- forms.py # Forms for user registration, login, game filtering
│ │-- bgg_api.py # Handles BoardGameGeek API integration
│ │-- templates/ # Stores HTML templates for rendering pages
│ │ │-- base.html # Base layout for all pages
│ │ │-- home.html # Homepage with search bar
│ │ │-- login.html # User login page
│ │ │-- register.html # User signup page
│ │ │-- game.html # Game details page
│ │ │-- dashboard.html # User dashboard
│ │ │-- admin/
│ │ │ │-- admin_dashboard.html # Admin dashboard
│ │ │ │-- manage_users.html # Admin user management
│ │ │ │-- manage_games.html # Admin game management
│ │-- static/ # Stores CSS, JavaScript, images
│ │ │-- css/
│ │ │ │-- style.css # Custom styles
│ │ │-- js/
│ │ │ │-- scripts.js # Interactive UI features
│ │-- utils.py # Helper functions for formatting, validation, etc.
│-- config.py # Configuration settings (database, API keys)
│-- run.py # Entry point for running the app
│-- requirements.txt # Dependencies
│-- README.md # Project documentation
│-- .env # Environment variables (DB connection, API keys)

🛠 Future Enhancements

👨‍🎓 AI Chatbot for game suggestions.

⚖️ User Ratings & Reviews for board games.

🎮 Game Night Planner to schedule and invite friends.
