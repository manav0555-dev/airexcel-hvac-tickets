# HVAC Complaint Ticketing System

A web-based complaint tracking system for HVAC servicing businesses. Track complaints against technicians across job sites, assign priorities, draw insights, and monitor repeat issues.

## Features

- **Complaint Management** — Create, assign, update, and close complaints with priority levels (1-5)
- **Priority Queue** — View complaints sorted by priority or FCFS (first come first served)
- **Technician Assignment** — Assign complaints to technicians; technicians see only their own tickets
- **Job Site Tracking** — Organize complaints by job site locations
- **Dashboard & Insights** — Visual breakdowns by priority, category, technician, and job site
- **Repeat Tracking** — Identify repeat complainants and technicians with high complaint counts
- **Notes & Activity Log** — Add notes to complaints for tracking progress
- **Role-Based Access** — Admin and Technician roles with different permissions

## Quick Start

```bash
# Install dependencies
pip install -r requirements.txt

# Run the app (initializes DB automatically)
python app.py

# Optionally load sample data
python seed_data.py
```

Open http://localhost:5000 in your browser.

## Default Login

- **Admin:** username `admin`, password `admin123`
- **Technicians (after seeding):** username `jsmith`/`mwilson`/`ljones`/`rbrown`/`akumar`, password `tech123`

## Tech Stack

- **Backend:** Python Flask
- **Database:** SQLite
- **Frontend:** Plain HTML/CSS/JavaScript (Jinja2 templates)

## Complaint Categories

Installation, Repair, Maintenance, Noise/Vibration, Temperature, Airflow, Leak, Electrical, Billing, Professionalism, Timeliness

## Priority Scale

| Level | Label    | Color  |
|-------|----------|--------|
| 1     | Critical | Red    |
| 2     | High     | Orange |
| 3     | Medium   | Yellow |
| 4     | Low      | Blue   |
| 5     | Minimal  | Gray   |
