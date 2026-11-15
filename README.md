# 💸 Smart Expense Tracker

A simple web app to **record expenses, categorize spending, and visualize monthly charts and budgets**.
Built with Python, Streamlit, Pandas and Matplotlib.

> Domain: Web Development / Data Analytics

---

## ✨ Features

- **Add expenses** with amount, category, date and note
- **Categorize spending** (Food, Transport, Shopping, Bills, Health, Entertainment, Other)
- **Monthly trend chart** compared against your total budget
- **Category breakdown** pie chart for any selected month
- **Budgets per category** with progress bars and warnings at 80% and when exceeded
- **Editable transaction table**: edit cells, add or delete rows, then save
- **CSV import / export** to bring in existing data or back it up
- **Persistent storage** in local CSV files (`expenses.csv`, `budgets.csv`)
- **Demo data** button to try the app instantly, and **Clear all** to start fresh

## 🛠 Tech Stack

| Tool | Purpose |
|---|---|
| Python 3.9+ | Core language |
| Streamlit | Web interface and forms |
| Pandas | Data cleaning, grouping, monthly aggregation |
| Matplotlib | Bar and pie charts |

## 📁 Project Structure

```
smart-expense-tracker/
├── app.py            # Streamlit application
├── requirements.txt  # Python dependencies
├── index.html        # Standalone browser version (no Python needed)
├── README.md
├── expenses.csv      # Created automatically on first save
└── budgets.csv       # Created automatically on first run
```

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/<your-username>/smart-expense-tracker.git
cd smart-expense-tracker
```

### 2. (Optional) Create a virtual environment

```bash
python -m venv venv
source venv/bin/activate        # Windows: venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the app

```bash
streamlit run app.py
```

Open **http://localhost:8501** in your browser.

## 📖 How to Use

1. Use the sidebar to **add an expense** (amount, category, date, note).
2. Set your **monthly budget** for each category in the sidebar.
3. Pick a **month** from the dropdown to see its totals, charts and budget status.
4. Scroll to the table to **edit or delete** transactions, then press **Save changes**.
5. Use **Download CSV** to export your data.

### CSV import format

```csv
Date,Category,Amount,Note
2026-11-02,Food,450,Groceries
2026-11-03,Transport,120,Metro
```

## 🌐 Deploy Online (Free)

1. Push this project to a public GitHub repository.
2. Go to [share.streamlit.io](https://share.streamlit.io) and sign in with GitHub.
3. Click **New app**, choose your repository, branch `main`, and main file `app.py`.
4. Click **Deploy** and share the generated link.

> Note: on Streamlit Community Cloud, saved CSV files may reset when the app restarts.
> Use **Download CSV** to back up your data, or connect a database for permanent storage.

## 🖥 Standalone Web Version

`index.html` is a no-install version of the tracker. Double-click it to open in any browser.
Data is stored in the browser's local storage. Charts need an internet connection (Chart.js is loaded from a CDN).

## 🔮 Future Improvements

- User login and multi-user support
- Bank statement / receipt import (OCR)
- Automatic categorization using machine learning
- Spending forecasts and savings goals
- Database backend (SQLite or PostgreSQL)

## 📄 License

This project is released under the MIT License. Feel free to use and modify it.
