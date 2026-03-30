# 💸 Expense Tracker MCP Server

An **AI-integrated Expense Tracker backend** built using the **FastMCP framework** and **SQLite**, designed to work as a tool-enabled server for AI agents.

This project enables AI systems (like LLMs) to **store, retrieve, and analyze financial data programmatically**.

---

## 🚀 Features

* ➕ Add expenses with category, subcategory, and notes
* 📋 List expenses within a date range
* 📊 Summarize expenses by category
* 🧠 AI-compatible via MCP (Model Context Protocol)
* 💾 SQLite database with async support using `aiosqlite`
* 📂 Dynamic categories resource (JSON-based)

---

## 🛠️ Tech Stack

* Python
* FastMCP
* SQLite
* aiosqlite (async DB operations)

---

## 📁 Project Structure

```
.
├── main.py              # MCP server implementation
├── categories.json     # Optional category configuration
└── README.md
```

---

## ⚙️ Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/expense-tracker-mcp.git
cd expense-tracker-mcp
```

### 2. Install Dependencies

```bash
pip install fastmcp aiosqlite
```

### 3. Run the Server

```bash
python main.py
```

Server will start at:

```
http://0.0.0.0:8000
```

---

## 🧩 MCP Tools

### ➤ Add Expense

```python
add_expense(date, amount, category, subcategory="", note="")
```

---

### ➤ List Expenses

```python
list_expenses(start_date, end_date)
```

---

### ➤ Summarize Expenses

```python
summarize(start_date, end_date, category=None)
```

Returns:

* Total spending per category
* Number of transactions

---

## 📦 MCP Resource

### Categories Endpoint

```
expense:///categories
```

* Returns predefined categories
* Falls back to default if JSON file is missing

---

## 🧠 Use Case

This project demonstrates how to:

* Build **AI-tool compatible backends**
* Enable **LLM agents to interact with structured databases**
* Combine **async Python + lightweight DB systems**
* Create **real-world AI automation tools**

---

## 🔮 Future Improvements

* User authentication
* Multi-user support
* Budget tracking & alerts
* Visualization dashboard (Streamlit / Power BI)
* API deployment (Docker + Cloud)

---

## 👨‍💻 Author

**Jatinpreet Singh Dhariwal**
 Data Analyst 

---

## ⭐ If you like this project

Give it a ⭐ on GitHub and feel free to contribute!
