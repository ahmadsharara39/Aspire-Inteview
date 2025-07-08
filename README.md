# Aspire-Inteview

Project Overview
The Inventory Management System is a web application that helps businesses keep track of their inventory. This project is built with React for the frontend and Flask for the backend, providing a simple and modern interface to manage inventory items. The system includes features like adding, editing, and deleting items, as well as basic AI-driven inventory reordering suggestions based on stock thresholds.

Features
Inventory Management: Add, edit, and delete inventory items (name, quantity, category, and status).

Search: Search for items by name, category, or status.

Reorder Suggestions: AI-based feature that suggests items to reorder when stock levels are low (using a predefined threshold).

Responsive Design: The app is fully responsive, optimized for both desktop and mobile devices.

Requirements
Frontend (React)
React: JavaScript library for building the user interface.

Axios: Promise-based HTTP client to make requests to the Flask backend.

Backend (Flask)
Flask: Python web framework for building the API endpoints.

Flask-CORS: To handle Cross-Origin Resource Sharing (CORS) for the React frontend.

Python
Python 3.x: Required to run the Flask server.

Project Setup
1. Frontend (React)
Install Dependencies
First, ensure that you have Node.js and npm installed. Then, navigate to the frontend folder in your project directory and install the required dependencies:
cd inventory-management
npm install

Run the React Development Server
Once the dependencies are installed, you can start the React development server:
npm start

2. Backend (Flask)
Install Python Dependencies
First, ensure that you have Python 3.x installed. Then, navigate to the backend folder and install the required dependencies using pip:
cd backend
pip install flask flask-cors
python app.py

How It Works
1. Frontend (React)
Inventory Management:

The frontend allows users to add, edit, and delete inventory items. It interacts with the backend via Axios to send and retrieve data from the Flask API.

Search Functionality:

Users can search for items by name, category, or stock status. The search feature is implemented using basic filtering on the frontend.

Reorder Suggestions:

The frontend fetches reorder suggestions from the Flask backend, which checks if any inventory items fall below the predefined threshold (e.g., quantity < 10).

2. Backend (Flask)
API Endpoints:

GET /api/items: Fetches all inventory items and reorder suggestions.

POST /api/items: Adds a new item to the inventory.

PUT /api/items/{id}: Edits an existing inventory item.

DELETE /api/items/{id}: Deletes an inventory item.

Reorder Suggestion Logic:

The backend includes a reorder suggestion feature that suggests items for restocking based on their quantity.
