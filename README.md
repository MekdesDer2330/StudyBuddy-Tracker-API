The **StudyBuddy Tracker API** is a backend service built with **Django REST Framework (DRF)** to help students track their study sessions by subject, duration, and focus level.  
It includes authentication, CRUD operations, and custom endpoints for daily and weekly summaries.
##  Features

- **User Authentication** – Sign up and log in securely  
- **Subjects Management (CRUD)** – Add, update, delete, and list study subjects  
- **Study Sessions (CRUD)** – Track sessions with duration and focus level  
- **Custom Endpoints**  
  - Today’s study sessions  
  - Weekly summary (total hours, average focus, etc.)  
##  Tech Stack

- [Python 3.x](https://www.python.org/)  
- [Django](https://www.djangoproject.com/)  
- [Django REST Framework](https://www.django-rest-framework.org/)  
- [SQLite / PostgreSQL](https://www.postgresql.org/) (database)  
- [PythonAnywhere](https://www.pythonanywhere.com/) (deployment target)  

## Project Structure (Planned)

studybuddy-tracker-api/
│── manage.py
│── requirements.txt
│── README.md
│── .gitignore
│── studybuddy/ # Main project folder
│ ├── settings.py
│ ├── urls.py
│ └── ...
│── tracker/ # App for subjects & study sessions
│ ├── models.py
│ ├── views.py
│ ├── serializers.py
│ └── urls.py

##  Installation & Setup

1. **Clone the repository**
   git clone https://github.com/MekdesDer2330/studybuddy-tracker-api.git
   cd studybuddy-tracker-api
Create and activate a virtual environment

python -m venv venv
source venv/bin/activate   # On Mac/Linux
venv\Scripts\activate      # On Windows
Install dependencies

pip install -r requirements.txt
Apply migrations

python manage.py migrate
Run the development server

python manage.py runserver
Open in browser: http://127.0.0.1:3000/

 API Testing
Use Postman or curl to test endpoints. Example:

# Get all subjects
GET http://127.0.0.1:3000/api/subjects/





Author
Mekdes Deriba
