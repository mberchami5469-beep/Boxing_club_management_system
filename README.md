# 🥊 Boxing Club Management System

A web application developed to manage boxers and their subscriptions in a boxing club.

This project was created as part of **TP4 – JavaScript**, with the objective of practicing data management using JSON, JavaScript modules, and DOM manipulation.

## 📌 Project Overview

The **Boxing Club Management System** is a simple web application that allows users to manage and visualize information about boxers, their categories, membership status, subscriptions, and payments.

## ✨ Features

- Display all registered boxers in a table.
- Search for boxers by name.
- Filter boxers by category.
- Filter active and inactive boxers.
- Display only boxers with at least one paid subscription.
- Calculate club statistics.
- Display the total amount of subscriptions.
- View boxer details and subscription history.
- Handle data loading errors.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| HTML5 | Structure of the application |
| CSS3 | Custom styling |
| Bootstrap | Responsive design and UI components |
| JavaScript ES6+ | Application logic and data processing |
| JSON | Data storage |

## 📂 Project Structure

```text
Boxing-Club-Management/
│
├── index.html
│
├── data/
│   ├── boxeurs.json
│   ├── offres.json
│   └── inscriptions.json
│
└── js/
    ├── state.js
    ├── dataService.js
    ├── selectors.js
    ├── view.js
    └── app.js
```

## ⚙️ Application Architecture

The application is organized into several JavaScript modules:

| File | Description |
|---|---|
| `state.js` | Stores application data and selected filters |
| `dataService.js` | Loads JSON files using Fetch API |
| `selectors.js` | Handles searching, filtering, and calculations |
| `view.js` | Displays data and statistics in the DOM |
| `app.js` | Initializes the application and manages user events |

## 🔍 Main Functionalities

### 1. Data Loading

The application loads three JSON files:

- `boxeurs.json`: Boxer information.
- `offres.json`: Club subscription offers and prices.
- `inscriptions.json`: Boxer registrations and payment statuses.

The Fetch API and async/await are used to retrieve the data.

### 2. Search and Filtering

Users can:
- Search for a boxer by name.
- Filter by category.
- Display active or inactive boxers.
- Show only boxers with paid subscriptions.

### 3. Subscription Management

The application connects boxers with their subscriptions using identifiers.

The subscription amount is calculated using:

`Total = Offer Price × Quantity`

Cancelled subscriptions are excluded from the total amount.

### 4. Statistics Dashboard

The application displays important club statistics:

- Total number of boxers.
- Number of active boxers.
- Number of paid subscriptions.
- Total subscription amount.

### 5. Boxer Details

Users can click the **View** button to access a boxer's information and subscription history.

## 💻 JavaScript Concepts Practiced

This project helped practice several important JavaScript concepts:

- **ES6 Modules:** `import` and `export`.
- **Fetch API:** Loading external JSON data.
- **Async/Await:** Managing asynchronous operations.
- **Array Methods:** `map()`, `filter()`, `find()` and `forEach()`.
- **DOM Manipulation:** `querySelector()`.
- **Event Handling:** `addEventListener()`.
- **Error Handling:** `try/catch`.
- **Application State:** Managing data and filters.

## 🚀 Installation and Execution

1. Clone the repository:

```bash
git clone YOUR_REPOSITORY_URL
```

2. Open the project folder:

```bash
cd Boxing-Club-Management
```

3. Open the project using Visual Studio Code.

4. Run the application using **Live Server**.

**Note:** Use a local server such as Live Server because the application uses `fetch()` to load JSON files.



## 👨‍💻 Author

**Mouad Berchami**

- Program: Licence Sciences et Techniques (LST)
- Speciality: Développement Informatique (DI)
- Group: 1
- Institution: Faculté des Sciences et Techniques de Marrakech (FST)

## 🎓 Academic Project

Developed as part of **TP4 – JavaScript**, focusing on JSON data management, modular JavaScript development, array manipulation, and DOM interaction.

---

⭐ If you find this project interesting, feel free to give it a star!
