# React-ratestore# Store Rating

A role-based Store Rating application where **System Administrators**, **Normal Users**, and **Store Owners** interact through dedicated dashboards.  
The platform ensures fair feedback, easy store discovery, and effective management with robust form validations and role-specific functionalities.

---

## About

**Store Rating** is a web application that enables:  
- **Users** to discover stores and submit ratings.  
- **Store Owners** to view store ratings and feedback.  
- **Administrators** to manage stores, users, and system activities.  

The application uses role-based access control to provide customized dashboards and permissions.

---

## Features

- Role-based login (Admin, User, Store Owner).  
- Store rating submission & modification.  
- Real-time dashboard insights.  
- Search and filter functionalities.  
- Secure authentication and form validations.  
- Separate dashboards for different user roles.  

---

## User Roles & Functionalities

### 👨‍💻 System Administrator
- Add new stores, normal users, and admin users.  
- Access dashboard displaying:  
  - Total number of users  
  - Total number of stores  
  - Total number of submitted ratings  
- Add new users with details:  
  - Name, Email, Password, Address  
- View store listings: Name, Email, Address, Rating.  
- View users list: Name, Email, Address, Role.  
- Apply filters on all listings (Name, Email, Address, Role).  
- View user details (Name, Email, Address, Role).  
  - If the user is a Store Owner, also view their store rating.  
- Logout functionality.  

### 👤 Normal User
- Signup & Login.  
- Signup form fields: Name, Email, Address, Password.  
- Update password after logging in.  
- View all registered stores.  
- Search stores by Name & Address.  
- Store listings include:  
  - Store Name  
  - Address  
  - Overall Rating  
  - User’s Submitted Rating  
  - Option to submit a rating  
  - Option to modify submitted rating  
- Submit ratings (1–5).  
- Logout functionality.  

### 🏪 Store Owner
- Login functionality.  
- Update password after logging in.  
- Dashboard includes:  
  - List of users who rated their store.  
  - Average store rating.  
- Logout functionality.  

---

## Form Validations

- **Name**: Min 20 characters, Max 60 characters.  
- **Address**: Max 400 characters.  
- **Password**: 8–16 characters, must include at least one uppercase letter and one special character.  
- **Email**: Must follow standard email validation rules.  

---

## Tech Stack

| Component         | Technology (Example)   |
|-------------------|-------------------------|
| Frontend          | React.js                |
| Backend           | Node.js + Express       |
| Database          | MySQL                   |
| Authentication    | JWT                     |
| Styling           | TailwindCSS / CSS       |
| Deployment        | Heroku / Vercel         |

*(Replace with your actual stack if different)*

---

## Screenshots

> All screenshots are stored in the `Screenshort/` folder of this repo.

| Page / Role | Screenshot |
|-------------|------------|
| Login | ![Login](Screenshort/login.png) |
| Signup | ![Signup](Screenshort/signup.png) |
| Admin Dashboard | ![Admin Dashboard](Screenshort/admin_dashboard.png) |
| User Dashboard | ![User Dashboard](Screenshort/user_dashboard.png) |
| Store Owner Dashboard | ![Store Owner Dashboard](Screenshort/storeowner_dashboard.png) |

---
## Getting Started

### Prerequisites
- Node.js v14+  
- npm or yarn  
- MySQL (or your DB)  
- Git  

---
### Installation
```bash
# clone repo
git clone https://github.com/ghorpadenakshatra47-commits/store-rating.git
cd store-rating

# install dependencies
npm install
Environment Variables
Create a .env file in root:

ini
Copy code
PORT=3000
DB_CONNECTION_STRING=your_database_uri
JWT_SECRET=your_jwt_secret
Running Locally
bash
Copy code
npm run dev
Visit http://localhost:3000

---
---

Usage
Users: Register, login, search for stores, submit/modify ratings.

Store Owners: Manage store ratings, view feedback.

Admins: Full system control (users, stores, ratings).

---
---

Contributing
Fork the repo.

Create a branch: git checkout -b feature/YourFeature.

Commit: git commit -m "Add new feature".

Push: git push origin feature/YourFeature.

Open a Pull Request.
---
---

License
Licensed under the MIT License. See the LICENSE file.

Contact
GitHub: ghorpadenakshatra47-commits

Project Link: Store Rating Repo

