# 🍽️ BizScout AI - Restaurant Location Analysis Tool

## 📋 Overview
BizScout AI is an intelligent tool that helps entrepreneurs and business owners identify optimal locations for their restaurants. By analyzing various factors including demographics, competition, and market potential, it provides data-driven insights for informed decision-making.

## ✨ Features
- **Smart Location Analysis**: Identifies optimal locations based on multiple factors
- **Risk-Capital Strategy**: Supports different investment strategies (High/Low Risk, High/Low Capital)
- **Interactive Maps**: Visual representation of potential locations with heat maps
- **Detailed Analytics**: Comprehensive analysis of location scores and distributions
- **Category-Based Analysis**: Insights specific to different restaurant categories

## 🚀 Getting Started

### Prerequisites
- Python 3.8 or higher
- pip (Python package installer)

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/bizscout-ai.git
   cd bizscout-ai
   ```

2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   # On Windows
   venv\Scripts\activate
   # On macOS/Linux
   source venv/bin/activate
   ```

3. Install required packages:
   ```bash
   pip install -r requirements.txt
   ```

### Running the Application
1. Start the Streamlit app:
   ```bash
   streamlit run streamlit_app.py
   ```

2. Open your browser and navigate to:
   ```
   http://localhost:8501
   ```

## 📊 Usage Guide

### 1. Select Operation Mode
- **Analyze Data**: Run analysis on existing data
- **Process Data**: Process new data
- **Process & Analyze**: Perform both operations

### 2. Choose Restaurant Category
Select from a list of standardized categories including:
- Mexican, Italian, Chinese, Japanese
- Fast Food, Pizza, Burgers
- Cafes, Coffee & Tea
- And more...

### 3. Set Risk-Capital Strategy
Choose your investment strategy:
- **Risk Level**: High Risk or Low Risk
- **Capital Level**: High Capital or Low Capital

### 4. View Results
The analysis provides:
- Interactive map with location heatmap
- Top location recommendations
- Score distribution analysis
- Category-based insights

## 📁 Project Structure
```
bizscout-ai/
├── data/
│   ├── raw/              # Raw data files
│   ├── processed/        # Processed data
│   └── final_output/     # Analysis results
├── src/
│   ├── data_processing/  # Data processing scripts
│   └── analysis/         # Analysis scripts
├── streamlit_app.py      # Main application
├── requirements.txt      # Dependencies
└── README.md            # Documentation
```

## 📂 Data Files Overview

### Raw Data (`data/raw/`)
- `la_zoning_1.csv` (371MB): Raw Los Angeles zoning data containing land use regulations and restrictions

### Semi-Processed Data (`data/semi_processed/`)
- `cluster_centroids.json` (70KB): Geographic coordinates for cluster centers
- `opentable_data_20250507_010741.csv` (930KB): Restaurant data from OpenTable
- `yelp_data_20250507_010740.csv` (15MB): Restaurant data from Yelp
- `zoning_data_20250507_010734.csv` (375MB): Processed zoning data with standardized formats

### Processed Data (`data/processed/`)
- `combined_restaurants_20250507_050351.csv` (1.4MB): Merged restaurant data from all sources with standardized categories

### Final Output (`data/final_output/`)
- `cluster_analysis_High_Capital_High_Risk.csv` (9.7KB): Analysis results for high capital, high risk strategy
- `cluster_analysis_High_Capital_Low_Risk.csv` (9.8KB): Analysis results for high capital, low risk strategy
- `cluster_analysis_Low_Capital_High_Risk.csv` (9.9KB): Analysis results for low capital, high risk strategy
- `cluster_analysis_Low_Capital_Low_Risk.csv` (9.9KB): Analysis results for low capital, low risk strategy

## 📝 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
