# AI-Powered Intelligent Load Balancing and Energy Distribution System for Smart Grids

## Project Overview

This project is a software-based smart grid simulation system that uses machine learning and optimization techniques to predict electricity demand and distribute available energy across different zones.

The system aims to improve energy allocation, monitor zone-level demand, and evaluate distribution performance.

## Key Features

- AI-based electricity demand forecasting using XGBoost.
- Intelligent load balancing and energy allocation.
- Priority-based energy distribution for critical zones.
- Zone management and monitoring.
- Demand prediction visualization.
- Grid simulation and performance monitoring.
- Alerts for grid conditions.
- Comparison of different energy allocation methods.
- Performance evaluation using fairness and satisfaction metrics.
- Interactive React dashboard.

## Technologies Used

**Backend**
- Python
- FastAPI
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Matplotlib

**Frontend**
- React
- Vite
- JavaScript
- CSS
- Chart.js

## Project Structure

```text
smart-grid-optimizer/
├── backend/
├── datasets/
├── frontend/
├── models/
├── reports/
├── requirements.txt
├── README.md
└── create_submission_zip.py
```

## Installation and Setup

### 1. Clone or extract the project

Extract the project ZIP file and open the project folder in PyCharm.

### 2. Create a Python virtual environment

```powershell
python -m venv .venv
```

### 3. Activate the environment

```powershell
.venv\Scripts\Activate.ps1
```

### 4. Install Python dependencies

```powershell
python -m pip install -r requirements.txt
```

## Running the Backend

Open a PyCharm terminal in the project root and run:

```powershell
python -m uvicorn backend.main:app --host 127.0.0.1 --port 8000 --reload
```

Backend API:
http://127.0.0.1:8000

API documentation:
http://127.0.0.1:8000/docs

## Running the Frontend

Open another PyCharm terminal:

```powershell
cd frontend
npm install
npm run dev
```

Open the local URL displayed by Vite in your browser.

## Machine Learning Model

The project uses an XGBoost-based model to forecast electricity demand using the available dataset and saved model files.

The prediction and optimization modules use these results to simulate energy allocation across different zones.

## Evaluation

The system includes evaluation modules for:

- Demand satisfaction.
- Zone-level allocation.
- Unmet energy demand.
- Fairness measurement.
- Comparison of allocation strategies.
- Multi-day simulation performance.

Generated evaluation results and charts are stored in the `reports/` directory.

## Important Note

This is an academic software simulation project. It uses prepared datasets and simulated energy supply and demand values. It is not connected to actual electrical infrastructure and does not perform real-world grid control.

## Conclusion

The project demonstrates how machine learning and optimization techniques can support intelligent energy distribution, load balancing, and performance analysis in a simulated smart grid environment.