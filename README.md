# Learning Progress Tracker

A Flask-based web application designed to help you monitor and track your daily learning activities and progress. This tool helps you stay organized and motivated in your learning journey by keeping track of your tasks, their completion status, and progress over time.

## Features

- Create and manage learning tasks
- Track completion status of learning activities
- Monitor your daily learning progress
- Update and modify learning goals
- Delete completed or outdated tasks
- Track task status (In Progress/Completed)
- Toggle task status with one click
- Color-coded status indicators
- Responsive and clean user interface
- SQLite database for data persistence

## Prerequisites

- Python 3.x
- Flask
- Flask-SQLAlchemy

## Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd <repository-name>
```

2. Create and activate a virtual environment (optional but recommended):
```bash
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate
```

3. Install the required packages:
```bash
pip install flask flask-sqlalchemy
```

## Setup

1. Initialize the database:
```bash
python init_db.py
```

2. Run the application:
```bash
python app.py
```

3. Open your web browser and navigate to:
```
http://localhost:5000
```

## Usage

- **Add a Learning Task**: Enter your learning activity or goal in the input field and click "Add Task"
- **Update a Task**: Click the "Update" link next to the task you want to modify
  - You can change both the task content and status
- **Delete a Task**: Click the "Delete" link next to the task you want to remove
- **Toggle Status**: Click the "Toggle" link next to the status to switch between "In Progress" and "Completed"

## Task Status

The application supports two task statuses:
- **In Progress** (default): Yellow badge indicating active learning tasks
- **Completed**: Green badge indicating finished learning activities

## Project Structure

```
├── app.py              # Main application file
├── init_db.py          # Database initialization script
├── static/
│   └── css/
│       └── main.css    # Stylesheet
├── templates/
│   ├── base.html       # Base template
│   ├── index.html      # Main page template
│   └── update.html     # Update task template
└── instance/
    └── test.db         # SQLite database file
```

## Database Schema

The Todo table includes the following fields:
- `id`: Primary key
- `content`: Learning task description
- `date_created`: Creation timestamp
- `status`: Task status (In Progress/Completed)

## Technologies Used

- **Backend**: Flask, SQLAlchemy
- **Database**: SQLite
- **Frontend**: HTML, CSS
- **Templating**: Jinja2

## Contributing

Feel free to submit issues and enhancement requests!

## License

This project is open source and available under the MIT License. 