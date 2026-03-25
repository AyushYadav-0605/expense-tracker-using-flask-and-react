#  Full-Stack Expense Tracker & Analytics Dashboard

A robust financial management application featuring a **Flask (Python) REST API** and a **React (Vite)** frontend. This project demonstrates the integration of relational databases with modern frontend data visualization.



##  Tech Stack
- **Frontend:** React.js, Vite, Recharts (Data Viz), CSS3
- **Backend:** Python, Flask, SQLAlchemy (ORM)
- **Database:** MySQL / SQLite
- **Tooling:** Git, REST API Testing

##  Technical Highlights: The "Refactor"
I took an existing baseline and performed a deep-dive technical audit to resolve several critical architectural bottlenecks:
- **Pagination Logic:** Refactored the backend SQL offset calculations to ensure 100% data visibility across paginated views.
- **Data Synchronization:** Resolved JSON key mismatches between the Flask API and React hooks to enable seamless monthly trend reporting.
- **Type-Safe Calculations:** Fixed JavaScript floating-point errors by implementing strict number casting for expense totals.
- **Soft-Delete Implementation:** Optimized the database query layer to correctly filter "deleted" records from the UI without losing historical data integrity.

##  Getting Started

### Backend
1. `cd backend`
2. `python -m venv venv && source venv/bin/activate`
3. `pip install -r requirements.txt`
4. `python app.py`

### Frontend
1. `cd frontend`
2. `npm install`
3. `npm run dev`

##  Future Roadmap
- [ ] Implement JWT-based User Authentication.
- [ ] Add CSV/PDF export functionality for monthly reports.
- [ ] Deploy to AWS/Render for live production access.
