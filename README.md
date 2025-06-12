# Flask Task Manager

A simple and elegant task management web application built with Flask and SQLite.

## Features

- Create new tasks
- View all tasks with their creation dates
- Update existing tasks
- Delete tasks
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

- **Add a Task**: Enter task description in the input field and click "Add Task"
- **Update a Task**: Click the "Update" link next to the task you want to modify
- **Delete a Task**: Click the "Delete" link next to the task you want to remove

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

## Technologies Used

- **Backend**: Flask, SQLAlchemy
- **Database**: SQLite
- **Frontend**: HTML, CSS
- **Templating**: Jinja2

## Contributing

Feel free to submit issues and enhancement requests!

## License

This project is open source and available under the MIT License. 