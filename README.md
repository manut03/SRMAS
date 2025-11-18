# Smart Restaurant Multi-Agent System (SRMAS)

## 📖 Overview
SRMAS is a lightweight, offline-capable **multi-agent system** designed for small restaurants, cafés, and food stalls.  
It automates **billing**, **inventory updates**, **sales logging**, and **restaurant analytics** using a clean multi-agent architecture.

This project demonstrates:
- Agent coordination (Billing, Inventory, Reports)
- Sequential + parallel agent flows
- Memory Bank (context storage)
- Session management
- CSV-based data layer (offline-friendly)
- Synthetic sales generation + advanced visual analytics

---

## 📂 Repository Structure

SRMAS/
│
├── notebook/
│ └── Smart_Restaurant_Multi-Agent_System_SRMAS.ipynb
│
├── data/
│ ├── menu.csv
│ ├── inventory.csv
│ └── sales.csv
│
├── images/ # Analytics visualizations (Cell 8)
│ ├── daily_sales_trend.png
│ ├── top_items.png
│ ├── category_pie.png
│ ├── bill_distribution.png
│ ├── sales_by_hour.png
│ └── srmas_architecture.png
│
└── README.md


---

## 🚀 Features

### ✔ Multi-Agent Architecture
- **Menu Agent** – menu retrieval & item info  
- **Billing Agent** – bill creation, sales logging  
- **Inventory Agent** – raw material deduction  
- **Report Agent** – daily summary & top-selling items  

### ✔ Memory & Session
- InMemorySessionService manages state  
- MemoryBank stores contextual notes for actions  

### ✔ Offline Data Layer (CSV)
- `menu.csv`  
- `inventory.csv`  
- `sales.csv`  

This makes SRMAS completely **offline and lightweight**.

### ✔ Agent Coordination
- Bill → Inventory update → Memory update → Reporting  
- Parallel inventory deductions using `asyncio.gather()`  

### ✔ Analytics (Cell 6 + Cell 8)
- Daily revenue plot  
- Distribution of bill amounts  
- Category-wise sales pie chart  
- Sales-by-hour trend  
- Top-selling items  
- Synthetic sales generation (150 orders)  

All graphs are stored in `/images`.

---

## 🧪 How to Run Locally

### 1. Clone the Repository
```bash
git clone https://github.com/manut03/SRMAS.git
cd SRMAS
