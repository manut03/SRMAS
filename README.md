# Smart Restaurant Multi-Agent System (SRMAS)

## 📖 Overview
SRMAS is a lightweight, offline-capable multi-agent system designed for small restaurants, cafés, and food stalls. It automates billing, inventory updates, sales logging, and generates restaurant analytics.

The system demonstrates:
- Multi-agent coordination (Billing, Inventory, Reporting)
- Sequential and parallel agent workflows
- CSV-based offline-friendly data layer
- Session management using InMemorySessionService
- Memory Bank for storing contextual notes
- Synthetic sales generation and advanced visual analytics

---

## 📂 Repository Structure

SRMAS/
├── notebook/
│   └── Smart_Restaurant_Multi-Agent_System_SRMAS.ipynb
│
├── data/
│   ├── menu.csv
│   ├── inventory.csv
│   └── sales.csv
│
├── images/
│   ├── daily_sales_trend.png
│   ├── top_items.png
│   ├── category_pie.png
│   ├── bill_distribution.png
│   ├── sales_by_hour.png
│   └── srmas_architecture.png
│
└── README.md

---

## 🚀 Features

### ✔️ Multi-Agent Architecture
- Menu Agent – retrieves menu items  
- Billing Agent – generates bills and logs sales  
- Inventory Agent – performs ingredient deduction  
- Report Agent – aggregates sales and generates analytics  

### ✔️ Session + Memory
- InMemorySessionService tracks session state  
- Memory Bank stores contextual insights from agent actions  

### ✔️ Offline CSV Data Layer
All data is stored locally:
- menu.csv  
- inventory.csv  
- sales.csv  

### ✔️ Agent Coordination Flow
Bill → Inventory Update → Memory → Reporting  
Inventory deductions run in parallel via `asyncio.gather()`.

### ✔️ Analytics (Notebook Cell 6 & 8)
The system generates:
- Daily revenue trend  
- Top-selling items  
- Category-wise sales distribution  
- Bill amount distribution  
- Sales-by-hour trend  

Output plots are saved inside the `images/` directory.

---

## 🧪 How to Run

### 1. Clone the Repository
git clone https://github.com/manut03/SRMAS.git
cd SRMAS

### 2. Install Dependencies
pip install pandas numpy matplotlib rich

### 3. Run the Notebook (Cells 1 → 8)
1. Install dependencies  
2. Generate synthetic menu and inventory  
3. Create base agent classes  
4. Implement concrete agents + Coordinator  
5. Generate demo orders  
6. Produce analytics  
7. Add evaluation + memory  
8. Produce synthetic sales + full analytics  

---

## 📊 Outputs You Will See
- Bill generation  
- Parallel inventory deductions  
- Sales appended to CSV  
- Daily and item-level analytics  
- Session memory logs  
- Multiple plots saved under images/  
- Evaluation score  

---

## 🖼️ Images Produced

images/srmas_architecture.png  
images/daily_sales_trend.png  
images/top_items.png  
images/category_pie.png  
images/sales_by_hour.png  
images/bill_distribution.png  

---

## 📘 License
This repository is distributed under CC BY-SA 4.0 (as required by the Kaggle competition).

---

## ⚠️ Notes
- No API keys required  
- All datasets are synthetic and safe to publish  
- Fully reproducible from a clean run  


