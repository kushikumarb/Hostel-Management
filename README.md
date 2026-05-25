# Stay-In: Hostel Management System 🏨

**Stay-In** is a responsive, web-based software solution designed to automate manual administrative tasks in student housing and hostel ecosystems. Developed during my internship at **Pentagon Space Pvt. Ltd., Bengaluru**, this platform replaces traditional paperwork with a clean, centralized system that coordinates data between hostel wardens (Administrators) and residents (Students).

---

## 🚀 Key Features

### 👤 Role-Based Portals & Authentication
* **Secure Onboarding:** Customized registration and login flows using secure credential handling.
* **Dual Dashboard Logic:** Distinct user experiences and routing paths for Admins vs. Students.

### ⚙️ Admin Capabilities
* **Live Analytics:** Instantly view active student counts, room occupancy status, and pending tasks.
* **Resource Management:** Seamlessly add, update, or remove rooms (Single/Double configurations) and set base rent prices.
* **Student Registry:** Maintain a clean digital database of registered students, complete with profile photos and ID proofs.
* **Financial Tracking:** Record monthly fee collections and flag pending dues.
* **Broadcast Board:** Create, update, or delete notifications on a global Notice Board.

### 🎓 Student Capabilities
* **Profile Management:** View allocated room details, registered profile settings, and payment summaries.
* **Interactive Notice Board:** Stay updated with real-time official announcements from the management.
* **Support & Maintenance Desk:** Log technical or living space complaints, tracking their status directly from the panel.

---

## 🛠️ Technology Stack

| Layer | Technology Used | Description |
| :--- | :--- | :--- |
| **Frontend** | HTML5, CSS3, JavaScript (ES6+) | Component-driven, responsive UI for Single Page Application (SPA) architecture. |
| **Backend** | Python, Django Framework | Robust Model-View-Template (MVT) server architecture managing business logic and API requests. |
| **Database** | MySQL | Highly organized relational database handling entity schemas and data integrity. |

---

## 💻 Installation & Setup Instructions

Follow these steps to run the complete environment locally on your machine.

### Prerequisites
* Python (v3.8 or higher)
* Node.js (v16 or higher)
* MySQL Server

### 1. Database Configuration
1. Open your MySQL client and run the following command to initialize a clean schema:
   ```sql
   CREATE DATABASE hostel_db;
Update your Django settings.py file under the DATABASES dictionary with your local MySQL password and user credentials.

2. Backend Setup (Django)
Navigate to your backend directory:

Bash
cd backend
Create and activate a virtual environment:

Bash
python -m venv venv
# On Windows:
venv\Scripts\activate
# On macOS/Linux:
source venv/bin/activate
Install dependencies and apply structural database migrations:

Bash
pip install django mysqlclient
python manage.py makemigrations
python manage.py migrate
Start the backend development server:

Bash
python manage.py runserver
The server will initialize at http://127.0.0.1:8000/.

3. Frontend Setup (ReactJS)
Navigate to your frontend project directory:

Bash
cd frontend
Install the necessary Node packages:

Bash
npm install
Boot up the user interface runtime environment:

Bash
npm start
The client interface will load automatically inside your browser at http://localhost:3000/.
