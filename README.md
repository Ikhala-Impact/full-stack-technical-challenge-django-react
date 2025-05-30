
# 🧪 Full-Stack Technical Challenge: Django + React

## 🎯 Objective
Build a small full-stack web application that displays sales data from a Django backend in a React frontend using a chart.

---

## 🔧 Backend (Django)

### 📁 Requirements
- Create a new Django project and app (e.g. `sales_dashboard` and `sales`).
- Create a model named `Sale` with the following fields:
  - `id` (auto)
  - `date` (DateField)
  - `amount` (FloatField)

### 📦 Data
- Set up a **local database** (e.g. PostgreSQL or SQLite) and connect it to your Django project.
- Populate the `Sale` table with the following data:

```python
[
    {"date": "2024-01-01", "amount": 1200.50},
    {"date": "2024-02-01", "amount": 950.75},
    {"date": "2024-03-01", "amount": 1320.20},
    {"date": "2024-04-01", "amount": 875.00},
    {"date": "2024-05-01", "amount": 1100.00},
    {"date": "2024-06-01", "amount": 980.25},
    {"date": "2024-07-01", "amount": 1035.40}
]
```

You can load this manually via a management command, script, or directly in a migration.

### 🌐 API
- Create a simple REST API endpoint that returns all sales in JSON format.
- Use Django REST Framework (DRF) or basic `JsonResponse`.

Expected response structure:

```json
[
  {
    "date": "2024-01-01",
    "amount": 1200.50
  },
  ...
]
```

---

## 🌐 Frontend (React)

### 🎨 Requirements
- Use any tooling you prefer (Vite, Create React App, etc.).
- Fetch the sales data from the Django backend.
- Render the data in a **line chart or bar chart** (e.g. using Recharts or Chart.js).
- Show the date on the X-axis and amount on the Y-axis.
- Add a title: **"Sales Overview"**

---

## ✅ Bonus (Optional)
- Allow the user to filter data by a date range.
- Format the amount in currency format (`R1,200.50`).
- Add a loading spinner while fetching data.

---

## 📦 Deliverables
- A GitHub repo with the backend and frontend in `/backend` and `/frontend` folders.
- A short README explaining:
  - How to run the backend and frontend
  - Any challenges you faced
  - What you’d improve next

---

## 💡 Extra Notes (Windows Compatibility and Setup)
This project is fully possible to complete on Windows. Some things to keep in mind:

### ✅ What Works Well
- **Django backend**: Python runs natively, and Django has no platform dependency.
- **Virtual environments**: Use `python -m venv venv` and activate with `venv\Scripts\activate`.
- **Django REST Framework**: Fully works.
- **React frontend**: Works fine via Node.js (just install Node and npm).
- **Charting libraries**: Recharts, Chart.js, etc., are OS-agnostic.
- **CORS configuration**: Same behavior on Windows.
- **Database**: SQLite works perfectly. PostgreSQL/MySQL also work.

### ⚠️ Common Challenges
- PATH issues (e.g. Python or npm not added correctly)
- Installing Python and enabling it in the terminal
- Dealing with CORS between localhost ports
- Serving React and Django concurrently
- Finding Windows-specific troubleshooting guides

📝 **Please document any technical challenges you face and how you solved them.**
