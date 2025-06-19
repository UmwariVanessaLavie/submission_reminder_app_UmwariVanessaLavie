# Submission Reminder App

This is a shell scripting project designed to help automate the process of identifying students who have not submitted their assignments and sending reminders. The application simulates a real-world Linux-based development workflow and is structured for scalability, clarity, and automation.

---

## Table of Contents

- [Project Overview](#project-overview)
- [Directory Structure](#directory-structure)
- [Setup Instructions](#setup-instructions)
- [Usage Instructions](#usage-instructions)
- [Copilot Script](#copilot-script)
- [Files and Scripts](#files-and-scripts)
- [Git Workflow](#git-workflow)
- [Learning Objectives](#learning-objectives)

---

## Project Overview

The Submission Reminder App performs the following:

- Automates the creation of the app environment
- Generates directories and scripts required for the reminder system
- Reads from a student submissions file to check who hasn’t submitted
- Prints reminder messages for pending submissions
- Allows users to update the assignment being tracked

---

## Directory Structure

After running the environment setup script, the following structure will be created:

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
├── startup.sh
└── image.png (optional)
```

---

## Setup Instructions

1. Clone the repository:
```bash
git clone https://github.com/<yourGitHubUsername>/submission_reminder_app_<yourGitHubUsername>.git
cd submission_reminder_app_<yourGitHubUsername>
```

2. Make the script executable:
```bash
chmod +x create_environment.sh
```

3. Run the setup script:
```bash
./create_environment.sh
```
This will prompt for your name and create the full directory structure with sample files.

---

## Usage Instructions

Once setup is complete, navigate to your project directory and run the app:

```bash
cd submission_reminder_<yourName>
./startup.sh
```

The app will:
- Load configuration from `config.env`
- Read from `submissions.txt`
- Identify and display students who haven’t submitted

---

## Copilot Script

To update the assignment name being tracked:

1. Make the copilot script executable:
```bash
chmod +x copilot_shell_script.sh
```

2. Run it:
```bash
./copilot_shell_script.sh
```

You will be prompted to enter a new assignment name, which updates the `ASSIGNMENT` in `config/config.env`, and re-runs the app to display reminders for the new assignment.

---

## Files and Scripts

### create_environment.sh
- Creates the full folder structure
- Populates necessary files with default content
- Makes all `.sh` files executable

### copilot_shell_script.sh
- Updates the assignment name in `config.env`
- Automatically re-runs the app

### startup.sh
- Runs the main logic in `reminder.sh`

### apps/reminder.sh
- Loads config
- Calls helper functions
- Reads `submissions.txt` and prints reminders

### modules/functions.sh
- Contains logic like `check_submissions`

### assets/submissions.txt
- CSV file with names, assignments, and statuses (add at least 5 students)

### config/config.env
- Contains environment variables like ASSIGNMENT and DAYS_LEFT

---

## Git Workflow

Your repository must follow this workflow:

- `feature/setup`: for rough work and development
- `main`: final version

Only these files should be in `main` when submitting:
- `create_environment.sh`
- `copilot_shell_script.sh`
- `README.md`

---

## Learning Objectives

- Master shell scripting basics
- Understand clean directory structure
- Write reusable functions in modular scripts
- Practice file handling, permission control, and automation
- Use Git branches for collaborative and organized development
- Document a full project using professional conventions

---

## Submission Guidelines

Repository Name:  
`submission_reminder_app_<yourGitHubUsername>`

Main Branch Must Contain Only:
- `create_environment.sh`
- `copilot_shell_script.sh`
- `README.md`

---

Created by: Umwari Vanessa  
© 2024 – All Rights Reserved
