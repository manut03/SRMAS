Smart Restaurant Multi-Agent System (SRMAS)
📌 Overview

SRMAS is a lightweight, offline-capable multi-agent system designed for small restaurants.
It automates:

Billing

Inventory updates

Sales logging

Restaurant analytics

The system uses four agents (Menu, Billing, Inventory, Reporting) orchestrated through a coordinator, supported by a session system and memory bank.
Data is stored using simple CSV files to keep the project easy to run anywhere—even offline.

📁 Repository Structure
SRMAS/
│
├── notebook/
│   └── smart-restaurant-multi-agent-system-srmas.ipynb   # Main project notebook
│
├── data/
│   ├── menu.csv
│   ├── inventory.csv
│   └── sales.csv
│
└── README.md

🚀 Features
✅ Multi-Agent Architecture

Menu Agent – reads menu.csv

Billing Agent – generates bills, appends sales.csv

Inventory Agent – updates inventory.csv

Report Agent – produces summaries & analytics

Memory Bank – stores contextual notes

Coordinator – orchestrates sequential + parallel flows

✅ Data Layer

Fully file-based (CSV)

Zero external dependencies

Offline-friendly

✅ Analytics & Visuals

The notebook produces multiple graphs using synthetic and real sales data:

Daily revenue trend

Top-selling items

Category-wise distribution

Hourly sales pattern

Bill amount distribution

These are useful for the Media Gallery in the Kaggle writeup.

🖼️ Images (Architecture + Analytics)

You can upload these images to GitHub or Kaggle as needed.

1. SRMAS Architecture Diagram
images/srmas_architecture.png

2. Daily Revenue Trend
images/daily_sales_trend.png

3. Top-Selling Items Bar Chart
images/top_items.png

4. Category-wise Sales Distribution
images/category_pie.png

5. Sales by Hour Trend
images/sales_by_hour.png

6. Bill Amount Distribution Histogram
images/bill_distribution.png

(Optional: Create an /images folder and upload the generated PNGs.)

🛠 How to Run
1. Open the Notebook

You can run SRMAS in:

Kaggle

Google Colab

Local Jupyter Notebook

2. Install dependencies
pip install pandas numpy matplotlib rich

3. Run all cells (1 → 8)

Cell 1: Dependencies

Cell 2: Create menu.csv + inventory.csv

Cell 3: Base agent classes

Cell 4: Concrete agents + Coordinator

Cell 5: Place demo orders

Cell 6: Basic analytics & memory logs

Cell 7: Evaluation

Cell 8: Synthetic sales + rich analytics (graphs)

📊 Outputs You’ll See

Bills generated from real flow

Inventory updates running in parallel

Sales appended to CSV

Daily summary

Top items summary

Multiple analytic graphs

Memory recall logs

Evaluation score

📘 License

This repository is distributed under CC BY-SA 4.0, as required by the Kaggle competition guidelines.

⚠️ Notes

No API keys are required or included.

All datasets are synthetic and safe to publish.

Fully reproducible: everything resets on a fresh run.
