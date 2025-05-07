# 📝 Permalist To-Do List with Node.js & PostgreSQL

This is a full-stack To-Do list application built using Node.js (with ES Modules), Express, PostgreSQL, and EJS. It allows users to add, edit, and delete tasks while saving all data in a PostgreSQL database. The app features a clean UI with inline editing and dynamic DOM rendering.

---

## 🔧 Features

- Add new tasks to your to-do list
- Inline edit existing tasks for easy updates
- Delete tasks with a checkbox for quick task removal
- Persistent database storage using PostgreSQL to save data
- Smooth and responsive user interface built with EJS templating and custom CSS

---

## 🧰 Tech Stack

- **Backend**: Node.js (with ES Modules), Express
- **Frontend**: EJS templating engine, HTML5, CSS3
- **Database**: PostgreSQL
- **Tools**: 
  - Body-parser (for handling POST request data)
  - Nodemon (optional, for automatic server restarting during development)

---

## 📂 Folder Structure

```
Todo-List/
├── public/              # Static files (CSS, icons, etc.)
│   └── styles.css
├── views/               # EJS views/templates
│   ├── partials/        # Header and footer components
│   │   ├── header.ejs
│   │   └── footer.ejs
│   └── index.ejs        # Main template for rendering tasks
├── app.js               # Express server & routes setup
├── package.json         # Project dependencies and scripts
├── .gitignore           # Git ignore file for unnecessary files
├── queries.sql          # SQL file to create the necessary database and tables
├── .env                 # Environment variables for database configuration
└── README.md            # Project documentation
```

---

## 🚀 Getting Started

Follow these steps to set up and run the Todo-List application locally:

### 1. Clone the repository

```bash
git clone https://github.com/Rishifanterboy/Todo-List.git
```

### 2. Install dependencies

Navigate into the project directory and run:

```bash
cd Todo-List
npm install
```

### 3. Set up PostgreSQL

Ensure you have PostgreSQL installed on your system. You can find the required SQL queries in the provided `queries.sql` file in the repository to set up the database and tables.

Run the following SQL commands in your PostgreSQL instance:

1. Create a new database:

```bash
createdb todolist
```

2. Run the SQL file to create tables and other necessary data:

```bash
psql -U your-username -d todolist -f queries.sql
```

### 4. Create a `.env` file

In the root of your project, create a `.env` file to store your PostgreSQL database credentials securely. The `.env` file should look like this:

```
 PG_USER=your-postgresql-username
 PG_HOST=your-host 
 PG_DATABASE=your-database-name
 PG_PASSWORD=your-postgresql-password
 PG_PORT=your-port-number

```

No additional steps are needed in the code; just make sure to set your .env file with the correct values and set the host to localhost in your .env file.

### 6. Run the application

Start the server:

```bash
npm start
```

If you're using Nodemon for automatic restarts during development, run:

```bash
npm run dev
```

Now, open your browser and go to [http://localhost:3000](http://localhost:3000). You can start adding, editing, and deleting tasks in your to-do list!

---

## 🎨 UI Design

The application features a clean, user-friendly interface for managing tasks. The tasks are displayed in a list format, where each task can be edited inline or deleted using a checkbox.

---

## 🧑‍💻 Usage

1. Visit the homepage at [http://localhost:3000](http://localhost:3000).
2. Add a new task by typing it into the input field and clicking the "Add Task" button.
3. Edit an existing task inline by clicking on the task text.
4. Mark tasks as complete or delete them using the respective buttons.

---
