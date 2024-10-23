# crime-complaint-management-system

## Overview

The Crime Complaint Management System is a web-based application designed to simplify and streamline the process of filing and tracking crime complaints. The system allows citizens to lodge complaints online, and provides police departments with a centralized platform to manage, track, and resolve those complaints effectively. The application ensures transparency, quick resolution of complaints, and enhances the communication between the public and law enforcement agencies.

## Features

- **User Registration & Login:** Secure registration and login for both citizens and police officers.
- **Lodge Complaint:** Citizens can submit detailed crime reports with evidence (images, documents, etc.).
- **Complaint Status Tracking:** Citizens can track the status of their complaints in real-time.
- **Admin Panel for Police:** Police can manage, review, and update complaints, assign tasks, and close cases.
- **Search & Filter:** Advanced search and filter options for complaints based on status, type, location, etc.
- **Notifications:** Automated email or SMS notifications to keep users informed about complaint progress.
- **Dashboard:** Admin and police officers have a dashboard showing active, pending, and resolved complaints.

## Technologies Used

- **Frontend:** HTML, CSS, JavaScript (React/Angular for single-page application behavior)
- **Backend:** Python (Flask/Django) or Node.js (Express)
- **Database:** MySQL / PostgreSQL / MongoDB
- **Authentication:** JWT (JSON Web Tokens) / OAuth 2.0
- **APIs:** RESTful APIs for complaint submission and tracking
- **Cloud Storage:** AWS S3 or Google Cloud Storage for media uploads (optional)

## Installation Guide

### Prerequisites
Make sure the following are installed on your system:

- Python 3.x or Node.js (depending on backend used)
- MySQL or PostgreSQL for database
- Git for version control

### Steps to Install

1. **Clone the Repository**
   ```bash
   git clone https://github.com/Kirandat/crime-complaint-management-system.git
   cd crime-complaint-management-system
   ```

2. **Install Backend Dependencies**
   - For Python/Flask/Django:
     ```bash
     pip install -r requirements.txt
     ```
   - For Node.js/Express:
     ```bash
     npm install
     ```

3. **Configure the Database**
   - Create a database in MySQL or PostgreSQL and update the database configuration in the project settings (`config.py` for Flask/Django or `.env` for Node.js).

4. **Run Database Migrations**
   - For Flask/Django:
     ```bash
     flask db upgrade  # Flask migration
     python manage.py migrate  # Django migration
     ```
   - For Node.js (if using Sequelize or ORM):
     ```bash
     npx sequelize db:migrate
     ```

5. **Run the Application**
   - For Python/Flask/Django:
     ```bash
     flask run  # Flask
     python manage.py runserver  # Django
     ```
   - For Node.js/Express:
     ```bash
     npm start
     ```

6. **Access the Application**
   - Open your browser and visit `http://localhost:5000` (for Flask/Django) or `http://localhost:3000` (for Node.js) to view the application.

### Frontend Setup (if applicable)
1. Navigate to the frontend folder (if it exists) and install dependencies:
   ```bash
   cd frontend
   npm install
   ```
2. Start the frontend application:
   ```bash
   npm start
   ```
   
   The frontend will usually run on `http://localhost:3000` or `http://localhost:4200` depending on your configuration.

## Usage

### For Citizens:
- Register an account and log in to access the system.
- Lodge a complaint by filling out the details of the crime.
- Upload any supporting documents or images.
- Check your dashboard to view your complaint status.

### For Police/Admin:
- Log in to access the police dashboard.
- Review complaints submitted by citizens.
- Assign officers to complaints and update their status.
- Use filters and search to prioritize cases effectively.

## Contributing

If you want to contribute to the development of the Crime Complaint Management System, follow these steps:

1. Fork the repository.
2. Create a new branch.
3. Make your changes and commit them.
4. Push the changes to your forked repository.
5. Submit a pull request for review.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
