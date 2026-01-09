Project Manager SPA
A modern, responsive Single Page Application for managing and tracking projects. Built with React, Vite, and Tailwind CSS.
Features

📋 Project List View - Display all projects in a clean, card-based layout
➕ Add New Projects - Dynamic form to create projects with title, description, status, date, and team
🔍 Real-time Search - Filter projects by title, description, or team name
🗑️ Delete Projects - Remove projects with a single click
📱 Responsive Design - Works seamlessly on desktop, tablet, and mobile devices
🎨 Modern UI - Contemporary design with smooth transitions and hover effects

Prerequisites
Before you begin, make sure you have the following installed:

Node.js (version 16 or higher)
npm (comes with Node.js)

To check if you have Node.js installed, run:
bashnode --version
npm --version
Installation

Clone or download this project to your local machine
Navigate to the project directory:

bash   cd project-manager

Install dependencies:

bash   npm install
This will install all required packages including React, Vite, Tailwind CSS, and Lucide icons.
Project Structure
Make sure your project has the following structure:
project-manager/
├── index.html              # Main HTML file (root level)
├── src/
│   ├── App.jsx            # Main React component
│   ├── index.jsx          # Application entry point
│   └── index.css          # Global styles with Tailwind
├── package.json           # Project dependencies
├── vite.config.js         # Vite configuration
├── tailwind.config.js     # Tailwind CSS configuration
├── postcss.config.js      # PostCSS configuration
└── .gitignore            # Git ignore file
Important: The index.html file must be in the root directory (same level as package.json), not in a public/ folder.
Running the Application
Development Mode
To start the development server:
bashnpm run dev
This will:

Start the Vite development server
Automatically open your browser to http://localhost:3000
Enable hot module replacement (changes appear instantly)

You should see output like:
VITE v5.x.x  ready in xxx ms
➜  Local:   http://localhost:3000/
If the browser doesn't open automatically, manually navigate to http://localhost:3000
Building for Production
To create a production-ready build:
bashnpm run build
This creates an optimized build in the dist/ folder.
Preview Production Build
To preview the production build locally:
bashnpm run preview
Usage

View Projects - The landing page displays all existing projects
Add a Project - Click the "New Project" button and fill out the form
Search Projects - Use the search bar to filter projects in real-time
Delete Projects - Click the trash icon on any project card to remove it

Troubleshooting
Page shows but no styling (looks bland)
Solution: Stop the server and reinstall dependencies:
bash# Press Ctrl+C to stop the server
npm install
npm run dev
Make sure you have tailwind.config.js and postcss.config.js in the root directory.
Port 3000 is already in use
Solution: Either:

Kill the process using port 3000, or
Change the port in vite.config.js:

javascript  server: {
    port: 3001,  // Change to any available port
    open: true
  }
index.html 404 error
Solution: Make sure index.html is in the root directory (same level as package.json), not in a public/ folder.
Module not found errors
Solution: Delete node_modules and reinstall:
bashrm -rf node_modules
npm install
Technologies Used

React 18 - UI framework
Vite - Fast build tool and dev server
Tailwind CSS - Utility-first CSS framework
Lucide React - Icon library
JavaScript (ES6+) - Programming language

Browser Support
This application works in all modern browsers:

Chrome/Edge (latest)
Firefox (latest)
Safari (latest)

License
This project is open source and available for educational purposes.# Lab-spa-with-react
