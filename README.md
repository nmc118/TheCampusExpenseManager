# TheCampusExpenseManager

## 📱 Overview
TheCampusExpenseManager is an Android expense management application designed for campus students and administrators. The app provides comprehensive expense tracking, budget management, and reporting features with role-based access control.

## ✨ Features

### For Students:
- 💰 **Expense Management**: Add, edit, delete, and view expenses
- 📊 **Category Management**: Organize expenses by categories
- 💵 **Budget Tracking**: Set and monitor monthly budgets
- 📈 **Reports**: View expense statistics and charts
- 👤 **User Profile**: Manage personal information
- 🔔 **Notifications**: Receive budget alerts and reminders

### For Admins:
- 👥 **User Management**: Create, edit, and manage user accounts
- 📊 **Category Management**: Manage global expense categories
- 📈 **System Reports**: View comprehensive expense reports across all users
- 🔧 **System Configuration**: Manage app settings and configurations

## 🛠️ Technology Stack
- **Language**: Java
- **IDE**: Android Studio
- **Minimum SDK**: API 24 (Android 7.0)
- **Target SDK**: API 34 (Android 14)
- **Database**: Room Database
- **Architecture**: MVVM (Model-View-ViewModel)
- **UI**: Material Design Components

## 📂 Project Structure
```
app/
├── src/main/
│   ├── java/com/thecampusexpensemanager/
│   │   ├── database/          # Room Database setup
│   │   ├── dao/               # Data Access Objects
│   │   ├── entity/            # Database entities
│   │   ├── repository/        # Repository layer
│   │   ├── viewmodel/         # ViewModels
│   │   ├── ui/
│   │   │   ├── auth/          # Login/Register activities
│   │   │   ├── admin/         # Admin dashboard and features
│   │   │   ├── student/       # Student dashboard and features
│   │   │   └── common/        # Shared UI components
│   │   └── utils/             # Utility classes
│   └── res/
│       ├── layout/            # XML layouts
│       ├── drawable/          # Images and icons
│       ├── values/            # Strings, colors, styles
│       └── menu/              # Menu resources
```

## 🚀 Getting Started

### Prerequisites
- Android Studio Arctic Fox or later
- JDK 8 or higher
- Android SDK API 24 or higher

### Installation
1. Clone the repository:
```bash
git clone https://github.com/nmc118/TheCampusExpenseManager.git
```

2. Open the project in Android Studio

3. Sync Gradle files

4. Run the app on an emulator or physical device

### Default Login Credentials
**Admin Account:**
- Username: `admin`
- Password: `admin123`

**Student Account:**
- Username: `student`
- Password: `student123`

## 📱 Screenshots
- Admin Dashboard: Manage users, categories, and view system-wide reports
- Student Dashboard: Track expenses, budgets, and view personal reports

## 🗄️ Database Schema

### User
- id (Primary Key)
- username
- password
- fullName
- email
- role (ADMIN/STUDENT)
- createdAt

### Expense
- id (Primary Key)
- userId (Foreign Key)
- categoryId (Foreign Key)
- amount
- description
- date
- createdAt

### Category
- id (Primary Key)
- name
- icon
- color
- createdBy (Foreign Key)

### Budget
- id (Primary Key)
- userId (Foreign Key)
- categoryId (Foreign Key)
- amount
- month
- year

## 📝 License
This project is created for educational purposes.

## 👨‍💻 Author
nmc118

## 🤝 Contributing
Contributions, issues, and feature requests are welcome!