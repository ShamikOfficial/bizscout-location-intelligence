# BizScout AI — Restaurant Location Intelligence

> **Scope note for reviewers:** Course / portfolio demo — compact sample. For interview depth, start with [agentic-trend-orchestrator](https://github.com/ShamikOfficial/agentic-trend-orchestrator) and [token-runway](https://github.com/ShamikOfficial/token-runway).

[![License: MIT](https://img.shields.io/badge/License-MIT-blue?style=flat-square)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.8+-blue?style=flat-square&logo=python&logoColor=white)]()

> Geo-intelligent recommendation system that helps entrepreneurs and analysts identify optimal restaurant locations in urban areas using demographics, competition, and market potential.

---

## Problem

Opening a restaurant in the wrong location is one of the costliest mistakes an entrepreneur can make. Site selection requires synthesizing zoning data, competitor density, demographics, and capital/risk tolerance — a multi-factor problem that spreadsheets alone cannot solve.

## Solution

BizScout AI scores and ranks candidate locations using clustering, heat maps, and category-specific analysis. Users choose a restaurant category and risk-capital strategy to get data-driven location recommendations on an interactive map.

## Key Results

| Feature | Detail |
|---------|--------|
| Data sources | LA zoning, Yelp, OpenTable restaurant data |
| Strategies | High/Low Risk × High/Low Capital combinations |
| Output | Interactive heat maps, top location rankings, score distributions |
| UI | Streamlit web app |

---

## Overview

BizScout AI is an intelligent tool that helps entrepreneurs and business owners identify optimal locations for their restaurants. By analyzing various factors including demographics, competition, and market potential, it provides data-driven insights for informed decision-making.

## Features

- **Smart Location Analysis** — Identifies optimal locations based on multiple factors
- **Risk-Capital Strategy** — Supports different investment strategies (High/Low Risk, High/Low Capital)
- **Interactive Maps** — Visual representation of potential locations with heat maps
- **Detailed Analytics** — Comprehensive analysis of location scores and distributions
- **Category-Based Analysis** — Insights specific to different restaurant categories

## Getting Started

### Prerequisites

- Python 3.8 or higher
- pip

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/ShamikOfficial/BizScout-AI.git
   cd BizScout-AI
   ```

2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   # Windows: venv\Scripts\activate
   # macOS/Linux: source venv/bin/activate
   ```

3. Install required packages:
   ```bash
   pip install -r requirements.txt
   ```

### Running the Application

```bash
streamlit run streamlit_app.py
```

Open `http://localhost:8501` in your browser.

## Usage Guide

### 1. Select Operation Mode
- **Analyze Data** — Run analysis on existing data
- **Process Data** — Process new data
- **Process & Analyze** — Perform both operations

### 2. Choose Restaurant Category
Mexican, Italian, Chinese, Japanese, Fast Food, Pizza, Burgers, Cafes, Coffee & Tea, and more.

### 3. Set Risk-Capital Strategy
- **Risk Level**: High Risk or Low Risk
- **Capital Level**: High Capital or Low Capital

### 4. View Results
- Interactive map with location heatmap
- Top location recommendations
- Score distribution analysis
- Category-based insights

## Project Structure

```
BizScout-AI/
├── data/
│   ├── raw/              # Raw data files
│   ├── processed/        # Processed data
│   └── final_output/     # Analysis results
├── src/
│   ├── data_processing/  # Data processing scripts
│   └── analysis/         # Analysis scripts
├── streamlit_app.py      # Main application
├── requirements.txt
└── README.md
```

## Data Files Overview

### Raw Data (`data/raw/`)
- `la_zoning_1.csv` — Los Angeles zoning data (land use regulations)

### Semi-Processed Data (`data/semi_processed/`)
- `cluster_centroids.json` — Geographic coordinates for cluster centers
- OpenTable and Yelp restaurant extracts
- Processed zoning data with standardized formats

### Final Output (`data/final_output/`)
- Cluster analysis CSVs for each risk-capital strategy combination

## License

MIT — see [LICENSE](LICENSE).
