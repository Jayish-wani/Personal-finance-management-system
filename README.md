# Expense Tracker

This is an Expense Tracker application built with React for the frontend and Node.js/Express for the backend. The app allows users to add, update, and delete their expenses, as well as view a list of expenses with the ability to filter them by month and year.It is a student target app in whicg the minimum limit is set to 500 and maximum is set to 15000, which can be changed accordingly , by this student can manage their monthly expense. Students found it difficult to manage their monthly expenses as they got a limited amount of money so by this they can manage accordingly, if the expense exceeds the limit of the budget it shows a pop up sign warning budget limit exceed.

 <img src="img 2077.jpg
  ">

## Table of Contents

- [Features](#features)
- [Installation](#installation)
  - [Backend Setup](#backend-setup)
  - [Frontend Setup](#frontend-setup)
- [Usage](#usage)
- [Error Handling and Loading States](#error-handling-and-loading-states)
- [API Endpoints](#api-endpoints)
- [Technologies Used](#technologies-used)

## Features

- Add new expenses
- Edit existing expenses
- Delete expenses
- View a list of expenses
- Filter expenses by month and year
- User authentication

## Installation

### Backend Setup

1. Clone the repository:
    ```bash
    git clone https://github.com/sukantadeveloper/expense-tracker.git
    cd expense-tracker
    ```

2. Install backend dependencies:
    ```bash
    cd backend
    npm install
    ```

3. Create a `.env` file in the `backend` directory and add the following environment variables:
    ```plaintext
    MONGO_URI=your_mongodb_connection_string
    JWT_SECRET=your_jwt_secret
    ```

4. Start the backend server:
    ```bash
    npm start
    ```

### Frontend Setup

1. Install frontend dependencies:
    ```bash
    cd frontend
    npm install
    ```

2. Start the frontend development server:
    ```bash
    npm start
    ```

## Usage

1. Open your browser and navigate to `http://localhost:3000` to view the application.
2. Use the form to add, edit, or delete expenses.
3. Filter expenses by selecting the desired month and year.

## Error Handling and Loading States

The application includes comprehensive error handling and loading state management to enhance user experience:

- **Error Handling**: 
  - Uses `react-toastify` for displaying error messages.
  - Catches and displays errors from API calls to inform the user of issues like failed deletions or updates.

- **Loading States**:
  - Shows loading indicators while fetching data, adding new expenses, updating existing ones, or deleting expenses.
  - Utilizes conditional rendering to display loaders during API requests.



## API Endpoints

### User Authentication Routes

- `POST /api/users/register` - Register a new user.
- `POST /api/users/login` - Login a user.

### Expense Routes

- `GET /api/expenses/:month/:year` - Fetch expenses for a specific month and year.
- `POST /api/expenses` - Add a new expense.
- `PATCH /api/expenses/:id` - Update an existing expense.
- `DELETE /api/expenses/:id` - Delete an expense.

## Technologies Used

- **Frontend**: React, Redux, TailwindCSS, react-toastify
- **Backend**: Node.js, Express, MongoDB, Mongoose
- **Authentication**: JWT


