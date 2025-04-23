# Mergington High School Activities

This project is a web application for managing extracurricular activities at Mergington High School. It allows students to view available activities, see the number of spots left, and sign up for activities using their email addresses. The application also displays a list of participants for each activity.

## Features

- **Activity List**: Displays all available activities with details such as description, schedule, and availability.
- **Sign-Up Form**: Allows students to sign up for activities by providing their email.
- **Participants Section**: Shows a list of participants already signed up for each activity.
- **Responsive Design**: Ensures the application looks good on both desktop and mobile devices.

## Technologies Used

- **Frontend**: HTML, CSS, JavaScript
- **Backend**: Python (FastAPI)
- **Styling**: Custom CSS for a clean and user-friendly interface

## How to Run

1. Ensure you have Python 3 and pip installed.
2. Install the required dependencies using `pip install -r requirements.txt`.
3. Run the application server.
4. Open the application in your browser to interact with it.

## API Endpoints

| Method | Endpoint                                                          | Description                                                         |
| ------ | ----------------------------------------------------------------- | ------------------------------------------------------------------- |
| GET    | `/activities`                                                     | Get all activities with their details and current participant count |
| POST   | `/activities/{activity_name}/signup?email=student@mergington.edu` | Sign up for an activity                                             |

## Data Model

The application uses a simple data model with meaningful identifiers:

1. **Activities** - Uses activity name as identifier:

   - Description
   - Schedule
   - Maximum number of participants allowed
   - List of student emails who are signed up

2. **Students** - Uses email as identifier:
   - Name
   - Grade level

All data is stored in memory, which means data will be reset when the server restarts.
