# DevOps-Work

This repository contains the core components and modules from the Task Management System for DevOps reference and deployment purposes.

## 📁 **Contents**

### **Core Directories**
- **`views/`** - EJS templates and UI components
  - `layout.ejs` - Main application layout
  - `tasks/` - Task-specific views (index, new, show)
  
- **`routes/`** - Express.js route handlers
  - `tasks.js` - Complete task management API routes
  
- **`config/`** - Database configuration files
  - `database.js` - MySQL database configuration
  - `database-sqlite.js` - SQLite database configuration
  
- **`node_modules/`** - Project dependencies

### **Key Files**
- **`package.json`** - Node.js dependencies and scripts
- **`.gitignore`** - Git ignore configuration

## 🚀 **Purpose**

This repository is designed for:
- **DevOps Reference** - Understanding the application structure
- **Component Reuse** - Extracting specific modules for other projects
- **Deployment Testing** - Isolated testing of core components
- **Documentation** - Reference implementation of Express.js patterns

## 🛠 **Technology Stack**

- **Backend**: Node.js, Express.js
- **Database**: SQLite, MySQL
- **Templating**: EJS
- **UI**: Bootstrap 5

## 📋 **Features Included**

### **Routes & API**
- Complete CRUD operations for tasks
- Advanced filtering and search
- Category and tag management
- Session management

### **Database Configurations**
- SQLite setup with sample data
- MySQL configuration for production
- Automatic database initialization

### **Views & Templates**
- Responsive Bootstrap UI
- Professional task management interface
- Advanced filtering components
- Statistics dashboard

## 🔧 **Setup Instructions**

1. **Install Dependencies**
   ```bash
   npm install
   ```

2. **Database Setup**
   - SQLite: Automatically configured
   - MySQL: Update `.env` with your credentials

3. **Start Application**
   ```bash
   npm start
   ```

## 📊 **Architecture Overview**

```
DevOps-Work/
├── views/                 # Frontend templates
│   ├── layout.ejs        # Main layout
│   └── tasks/            # Task views
├── routes/               # Backend logic
│   └── tasks.js          # Task routes
├── config/               # Database setup
│   ├── database.js      # MySQL config
│   └── database-sqlite.js # SQLite config
├── node_modules/         # Dependencies
├── package.json          # Project config
└── README.md            # This file
```

## 🌟 **Key Components**

### **Database Layer**
- Dual database support (SQLite/MySQL)
- Automatic schema creation
- Sample data seeding

### **API Layer**
- RESTful endpoints
- Comprehensive error handling
- Input validation

### **Presentation Layer**
- Responsive design
- Interactive components
- Professional UI/UX

## 📝 **Usage Examples**

### **Using the Routes**
```javascript
const taskRoutes = require('./routes/tasks');
app.use('/tasks', taskRoutes);
```

### **Database Configuration**
```javascript
const db = require('./config/database-sqlite');
// or
const db = require('./config/database');
```

### **View Templates**
```ejs
<%- include('layout') %>
<div class="container">
  <!-- Your content here -->
</div>
```

## 🔗 **Related Projects**

- **Main Project**: [Simple-Task-Management-System](https://github.com/AnuragBodkhe/Simple-Task-Management-System)
- **Live Demo**: Available on the main repository

---

**Note**: This repository contains core components extracted from the main Task Management System for modular development and DevOps purposes.