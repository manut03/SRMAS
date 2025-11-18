# Smart Restaurant Multi-Agent System (SRMAS)

## Overview
SRMAS is a lightweight, offline-capable multi-agent system designed for small restaurants, cafés, and food stalls.  
It automates billing, inventory updates, sales logging, and analytics using a modular multi-agent architecture.

This project demonstrates:
- Agent coordination (Billing, Inventory, Reports)
- Sequential and parallel agent flows
- Memory Bank (context storage)
- Session management
- CSV-based offline data layer
- Synthetic sales generation and visual analytics

---

## Repository Structure

SRMAS/
│
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

## Features

### Multi-Agent Architecture
- Menu Agent – retrieves menu and item details
- Billing Agent – creates bills and logs sales
- Inventory Agent – deducts ingredients
- Report Agent – generates summaries and analytics

### Memory and Session
- InMemorySessionService manages session state
- MemoryBank stores contextual notes

### Offline CSV-Based Data Layer
- menu.csv  
- inventory.csv  
- sales.csv  

### Agent Coordination Flow
Bill → Inventory Update → Memory Update → Reporting  
Parallel inventory deduction using asyncio.gather()

### Analytics (Notebook Cell 6 and 8)
The notebook generates:
- Daily revenue plot
- Top-selling items bar chart
- Category-wise sales pie chart
- Sales-by-hour trend
- Bill distribution histogram

Images are saved in the /images directory.

---

## How to Run

### 1. Clone the Repository
```bash
git clone https://github.com/manut03/SRMAS.git
cd SRMAS
```

### 2. Install Dependencies
```bash
pip install pandas numpy matplotlib rich
```

### 3. Run the Notebook (Cells 1 → 8)
1. Install dependencies  
2. Create synthetic menu and inventory  
3. Base agent classes  
4. Concrete agents and Coordinator  
5. Generate demo orders  
6. Basic analytics  
7. Evaluation and memory logging  
8. Synthetic sales and advanced analytics  

---

## Outputs
- Bill generation with line items
- Parallel inventory deductions
- Sales logging to CSV
- Daily summary and analytics
- Memory logs
- Multiple plots saved in images/
- Evaluation scores

---

## Images Produced
- images/srmas_architecture.png
- images/daily_sales_trend.png
- images/top_items.png
- images/category_pie.png
- images/sales_by_hour.png
- images/bill_distribution.png

---

## License
This repository is released under the CC BY-SA 4.0 license (as required by the Kaggle competition).

---

## Notes
- No API keys used
- All datasets are synthetic and safe to publish
- Notebook is fully reproducible from scratch

