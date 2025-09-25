# Course Evaluation Analysis Project

This project analyzes lecturer and course evaluation data from student feedback surveys. The analysis provides insights into course delivery, lecturer performance, and student satisfaction across different academic programs.

## Project Overview

The project processes course evaluation data containing:
- Student feedback on course delivery and lecturer performance
- Ratings across multiple evaluation criteria (content coverage, clarity, organization, etc.)
- Course and lecturer information
- Student agreement levels on various teaching aspects

## Data Structure

The evaluation data includes:
- **Course Information**: Course codes, titles, and levels of study
- **Lecturer Details**: Names and teaching assignments
- **Section 2 Ratings**: 19 evaluation criteria on course delivery (Excellent/Good/Satisfactory/Fair scale)
- **Section 3 Agreements**: 11 statements on teaching effectiveness (Strongly Agree/Agree/Disagree scale)
- **Comments**: Qualitative feedback from students

## Key Analysis Features

### 1. Data Processing
- Cleans and standardizes column names
- Maps text ratings to numerical scores for analysis
- Handles lecturer name variations and duplicates
- Filters out invalid or incomplete responses

### 2. Performance Analytics
- **Course Performance**: Rankings based on average delivery scores
- **Lecturer Effectiveness**: Individual lecturer performance metrics
- **Sentiment Analysis**: Converts qualitative ratings to quantitative scores
- **Course Load Analysis**: Number of courses per lecturer

### 3. Visualizations
- Top-performing courses by delivery and engagement scores
- Lecturer performance comparisons
- Course load distribution among faculty
- Trend analysis across different evaluation criteria

## Technical Implementation

### Dependencies
```python
pip install pandas numpy matplotlib jupyter fuzzywuzzy
```

### Key Components
- **Data Cleaning**: Standardizes survey responses and handles missing data
- **Scoring System**: Maps categorical responses to numerical values
- **Aggregation**: Groups data by course and lecturer for comparative analysis
- **Visualization**: Creates charts showing performance rankings and distributions

## System Setup

### Environment Setup
```bash
# Ubuntu/Debian (if python3.8 package exists)
sudo apt update
sudo apt install -y python3.8 python3.8-venv python3.8-dev build-essential

# create venv
python3.8 -m venv ex00
# activate
source ex00/bin/activate

# install required packages
pip install --upgrade pip
pip install pandas numpy jupyter matplotlib fuzzywuzzy

# save packages
pip freeze > requirements.txt
```

### Launch Jupyter Notebook
From your activated ex00 environment:
```bash
# recommended: run Jupyter without token (local dev only) or keep token for security
jupyter notebook --port=8891 --no-browser
# or if you prefer JupyterLab:
jupyter lab --port=8891 --no-browser
```

- Open http://localhost:8891 in your browser
- Open the existing `Notebook.ipynb` file to run the analysis

## Usage

1. **Data Input**: Place your course evaluation CSV file in the project directory
2. **Run Analysis**: Execute the Jupyter notebook cells to process the data
3. **View Results**: Review generated visualizations and performance rankings
4. **Export Insights**: Use the processed data for institutional reporting

## Output Metrics

- **Top 10 Courses**: Ranked by student satisfaction and delivery effectiveness
- **Lecturer Performance**: Individual scores across all evaluation criteria
- **Course Load Distribution**: Faculty workload analysis
- **Trend Analysis**: Performance patterns across different course levels and departments

## Data Privacy

This analysis tool is designed for institutional use to improve educational quality. Ensure compliance with data protection regulations when handling student feedback data.