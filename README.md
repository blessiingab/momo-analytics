# MoMo Analytics

GROUP8

 Project Description
This project processes MoMo SMS data in XML format.  
It extracts, cleans, and categorizes transactions, stores them in a relational database (SQLite for now), and generates data for dashboards.  
The frontend interface allows users to analyze and visualize the data with charts and tables.  

Key components:
- TL pipeline: Parse XML → Clean & Normalize → Categorize → Load to database
- Database: SQLite (relational storage of transactions)
- Frontend: HTML, CSS, JS dashboard for analytics and visualization
- Optional API: FastAPI endpoints to serve transaction and analytics data

## Team Members
 Blessing Ingabire – [blessiingab]
 
 Tabitha Dorcas Akimana – [tdorcas-akim]  
 Adoleh Samuel – [AdolehSamuel]


## Scrum Board
[Add your Scrum board link here – GitHub Projects / Trello / Jira]

## Architecture Diagram
See `/docs/architecture-diagram.png` for the system architecture.

## Project Structure (Planned)
├── README.md
├── .env.example
├── requirements.txt
├── index.html
├── web/
│ ├── styles.css
│ ├── chart_handler.js
│ └── assets/
├── data/
│ ├── raw/
│ ├── processed/
│ ├── db.sqlite3
│ └── logs/
├── etl/
│ ├── config.py
│ ├── parse_xml.py
│ ├── clean_normalize.py
│ ├── categorize.py
│ ├── load_db.py
│ └── run.py
├── api/
│ ├── app.py
│ ├── db.py
│ └── schemas.py
├── scripts/
│ ├── run_etl.sh
│ ├── export_json.sh
│ └── serve_frontend.sh
└── tests/
├── test_parse_xml.py
├── test_clean_normalize.py
└── test_categorize.py
