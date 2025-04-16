# Submission Reminder App

This project automates the creation of an environment for a submission reminder app. The app checks students' assignment submission statuses and generates reminders for those who have not submitted their work. It is implemented using shell scripting and follows a structured approach for better maintainability and scalability.

## Table of Contents
- [Project Overview]
- [Directory Structure]
- [Setup Instructions]
- [Usage Instructions]
- [Files and Scripts Explained]
- [Contributingripts Explained]

## Project Overview

This project automates:
1. Setting up a structured environment for the submission reminder app.
2. Creating necessary directories and files.
3. Checking a file containing student submission statuses.
4. Generating reminders for students who have not submitted their assignments.

### Key Features:
- **Automated Environment Setup**: The `create_environment.sh` script sets up the required directories and files.
- **Student Submission Check**: Reads a file to check if students have submitted their assignments.
- **Reminder Notifications**: Generates reminders for students who have not submitted their assignments.

## Directory Structure

The project is organized in the following structure:

```
submission_reminder_<yourName>/
├── apps/
│   └── reminder.sh
├── modules/
│   └── functions.sh
├── assets/
│   └── submissions.txt
├── config/
│   └── config.env
└── startup.sh
```

### Explanation of Directories and Files:
- **`apps/`**: Contains the main script file (`reminder.sh`) for checking submissions.
- **`modules/`**: Contains helper functions (`functions.sh`) used for checking student submissions.
- **`assets/`**: Contains data files like `submissions.txt`, listing students and their submission statuses.
- **`config/`**: Stores configuration files such as `config.env` which contains environment variables.
- **`startup.sh`**: Initializes the app and runs the `reminder.sh` script.

## Setup Instructions

To set up the environment for this project, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/<your-github-username>/submission_reminder_app.git
   cd submission_reminder_app
   ```

2. **Make the script executable**:
   ```bash
   chmod +x create_environment.sh
   ```

3. **Run the `create_environment.sh` script**:
   ```bash
   ./create_environment.sh
   ```
   This script will:
   - Prompt for your name and create a directory (`submission_reminder_<yourName>`).
   - Generate necessary subdirectories and files.
   - Populate `submissions.txt` with sample data.
   - Populate `functions.sh` with logic to check submissions.
   - Configure `config.env` with environment variables.

## Usage Instructions

Once the environment is set up, follow these steps to run the application:

1. **Run the app**:
   ```bash
   ./startup.sh
   ```

2. **View reminders**:
   The app will check the student submission statuses and print out reminders for students who have not submitted their assignments.

## Files and Scripts Explained

### `create_environment.sh`
- Automates the creation of directories and files necessary for the Submission Reminder App.
- Prompts for a name and sets up the required environment structure.
- Ensures all scripts are executable.

### `config/config.env`
- Stores environment variables such as the assignment name and the number of days remaining for submission.

### `apps/reminder.sh`
- The main script that:
  - Loads environment variables.
  - Calls functions from `functions.sh`.
  - Reads `submissions.txt` and checks which students have not submitted their assignments.

### `modules/functions.sh`
- Contains the `check_submissions` function that:
  - Reads `submissions.txt`.
  - Compares assignments with the configured assignment.
  - Prints reminders for students who have not submitted their work.

### `assets/submissions.txt`
- A CSV file containing student records with their names, assignments, and submission statuses.
- Used to generate reminder notifications.

### `startup.sh`
- Navigates to the correct directory and runs `reminder.sh` to execute the reminder logic.

## Contributing

If you would like to contribute to this project, follow these steps:

1. Fork the repository.
2. Create a new branch for your changes.
3. Commit your changes and push them to your fork.
4. Open a pull request with a description of the changes.

