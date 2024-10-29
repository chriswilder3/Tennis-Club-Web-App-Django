# 🎾 Tennis Club Web App

A Django-based web application for managing and displaying a tennis club's member information, events, and activities. This project allows club administrators and visitors to view details of club members, filter them by specific attributes, and explore various club-related pages.

## 📌 Features

- **Member Directory**: Lists all registered club members with links to view their personal details.
- **Individual Member Profiles**: Detailed view of each member, displaying personal information such as name, phone number, and date of joining.
- **Dynamic Filtering**: Search and filter members by specific criteria, like names that start with a certain letter.
- **Customizable Templates**: Template-based front-end with `HTML` and `Django Template Language` for easy content customization and integration.

## 🚀 Getting Started

### Prerequisites
- Python 3.x
- Django 3.x or later

### Installation
1. **Download and Extract the Zip File**: 
   - Download `tennis_club.zip` and extract it into your preferred project directory.

2. **Set Up a Virtual Environment**:
   - Create and activate a virtual environment:
     ```bash
     python -m venv venv
     source venv/bin/activate  # On Windows, use venv\Scripts\activate
     ```

3. **Install Dependencies**:
   - Install the required dependencies specified in the `requirements.txt` file:
     ```bash
     pip install -r requirements.txt
     ```

4. **Run Migrations and Start the Server**:
   - Set up the database and start the Django development server:
     ```bash
     python manage.py migrate
     python manage.py runserver
     ```

5. **Access the Application**:
   - Open your browser and go to `http://127.0.0.1:8000/` to view the Tennis Club site.

## Project Structure

- **urls.py**: Defines URL routing and maps each route to corresponding views.
- **views.py**: Contains view functions for rendering pages, querying member data, and handling specific requests.
- **templates/**: Stores all HTML templates for rendering pages.
- **models.py**: Defines the `Member` model to store member data.

### Folder Structure
```plaintext
tennis_club/
├── members/
│   ├── migrations/
│   ├── templates/
│   │   ├── show_members.html
│   │   ├── member_details.html
│   │   ├── main.html
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── models.py
│   ├── tests.py
│   └── views.py
├── tennis_club/
│   ├── __init__.py
│   ├── asgi.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
├── requirements.txt
└── manage.py
