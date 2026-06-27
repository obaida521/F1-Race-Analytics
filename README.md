# 🏎️ F1 Race Strategy Analytics System

## 🚀 Project Overview

The **F1 Race Strategy Analytics System** is an AI-assisted race engineering platform designed to simulate real-world Formula 1 pit wall decision-making.

The system processes telemetry data including tyre degradation, fuel consumption, ERS deployment, lap pace trends, track position, and race conditions to generate intelligent strategy recommendations using advanced analytics and Google Gemini AI.

This project replicates the analytical workflow used by professional Formula 1 race engineers to support strategic decisions during race sessions.

---

## 🎯 Key Capabilities

### 📊 Telemetry Analytics

* Real-time telemetry monitoring
* Lap-by-lap performance evaluation
* Pace delta analysis
* Sector performance assessment

### 🛞 Tyre Intelligence

* Tyre wear prediction
* Degradation trend analysis
* Compound performance comparison
* Optimal pit window calculation

### ⛽ Fuel Management

* Fuel consumption analytics
* Lift-and-coast recommendations
* Aggressive vs Balanced fuel modes
* Fuel-saving strategy generation

### ⚡ ERS Optimization

* ERS deployment monitoring
* Energy harvesting efficiency analysis
* Battery usage optimization
* Deployment strategy recommendations

### 🏁 Pit Stop Strategy Engine

* Undercut opportunities
* Overcut opportunities
* Pit window predictions
* Strategy viability comparison

### 🤖 AI Race Engineer

* Google Gemini-powered recommendations
* Natural language race insights
* Human-like engineering feedback
* Strategic risk assessment

### 🔬 What-If Simulation Engine

* Safety Car scenarios
* Virtual Safety Car scenarios
* Alternative tyre strategies
* Pit stop timing simulations

---

# 🏗️ System Architecture

```text
Telemetry Data
      │
      ▼
┌─────────────────────────────┐
│      Analytics Layer        │
├─────────────────────────────┤
│ Telemetry Analyzer          │
│ Fuel Analyzer               │
│ ERS Analyzer                │
│ Strategy Comparator         │
│ Simulation Analyzer         │
└─────────────────────────────┘
      │
      ▼
┌─────────────────────────────┐
│ Recommendation Engine       │
└─────────────────────────────┘
      │
      ▼
┌─────────────────────────────┐
│ Google Gemini AI            │
│ (via OpenRouter API)        │
└─────────────────────────────┘
      │
      ▼
┌─────────────────────────────┐
│ FastAPI Backend Services    │
└─────────────────────────────┘
      │
      ▼
┌─────────────────────────────┐
│ Next.js Dashboard           │
└─────────────────────────────┘
```

---

# 🛠️ Technology Stack

## Backend

| Technology  | Purpose                |
| ----------- | ---------------------- |
| Python 3.11 | Core Development       |
| FastAPI     | REST API Development   |
| NumPy       | Mathematical Analytics |
| Pandas      | Data Processing        |
| Uvicorn     | API Server             |

## AI & Machine Learning

| Technology       | Purpose                  |
| ---------------- | ------------------------ |
| Google Gemini AI | Strategy Recommendations |
| OpenRouter API   | AI Gateway               |
| Langflow         | Visual AI Workflow       |

## Frontend

| Technology    | Purpose            |
| ------------- | ------------------ |
| Next.js 14    | Frontend Framework |
| TypeScript    | Type Safety        |
| Tailwind CSS  | UI Styling         |
| Framer Motion | Animations         |

## DevOps

| Technology | Purpose         |
| ---------- | --------------- |
| GitHub     | Version Control |
| Render     | Deployment      |
| Postman    | API Testing     |
| VS Code    | Development     |

---

# 📂 Project Structure

```text
F1-Race-Analytics
│
├── analytics
│   │
│   ├── telemetry_analysis
│   │   └── analyzer.py
│   │
│   ├── fuel_analysis
│   │   └── fuel_analyzer.py
│   │
│   ├── ers_analysis
│   │   └── ers_analyzer.py
│   │
│   ├── strategy_insights
│   │   └── strategy_comparator.py
│   │
│   ├── simulation_analytics
│   │   └── simulation_analyzer.py
│   │
│   ├── recommendation_engine
│   │   └── recommender.py
│   │
│   ├── granite_integration
│   │   └── gemini_client.py
│   │
│   └── main.py
│
├── data
│   └── sample_telemetry.json
│
├── requirements.txt
├── .gitignore
└── README.md
```

---

# ⚙️ Installation

## Clone Repository

```bash
git clone https://github.com/obaida521/F1-Race-Analytics.git
cd F1-Race-Analytics
```

## Create Virtual Environment

```bash
python -m venv venv
```

### Windows

```bash
venv\Scripts\activate
```

### Linux / macOS

```bash
source venv/bin/activate
```

## Install Dependencies

```bash
pip install -r requirements.txt
```

## Configure Environment Variables

Create a `.env` file:

```env
OPENROUTER_API_KEY=your_api_key_here
```

## Start Server

```bash
python -m uvicorn analytics.main:app --reload
```

Open:

```text
http://localhost:8000/docs
```

---

# 📡 REST API Endpoints

| Method | Endpoint                | Description         |
| ------ | ----------------------- | ------------------- |
| GET    | /                       | Service Status      |
| GET    | /health                 | Health Check        |
| GET    | /api/telemetry/snapshot | Telemetry Data      |
| POST   | /analyze                | Full Race Analysis  |
| POST   | /simulate               | Scenario Simulation |
| POST   | /pace-analysis          | Pace Analytics      |

---

# 📈 Sample Analysis Output

```json
{
  "lap": 18,
  "recommended_strategy": "tyre_saving",
  "pit_window": "19-21",
  "fuel_mode": "save",
  "ers_strategy": "balanced",
  "risk_level": "medium",
  "recommendation": "Pit within next 3 laps. Tyre degradation increasing rapidly."
}
```

---

# 🔀 Langflow Workflow

```text
Telemetry Snapshot
        │
        ▼
JSON Processing
        │
        ▼
Prompt Builder
        │
        ▼
Google Gemini AI
        │
        ▼
Race Engineer Recommendation
```

---

# 🎯 Future Enhancements

* Live telemetry streaming
* Multi-car comparison dashboard
* Driver performance analytics
* Predictive race outcome modeling
* AI-powered pit strategy optimizer
* IBM Granite integration
* Historical race data analytics
* Interactive race simulator

---

# 📊 Skills Demonstrated

This project showcases expertise in:

* Artificial Intelligence
* Generative AI
* Data Analytics
* FastAPI Development
* Telemetry Processing
* Strategy Optimization
* Statistical Analysis
* REST API Design
* Prompt Engineering
* Langflow Workflows
* Software Architecture
* Full Stack Development

Licensed under the MIT License.
