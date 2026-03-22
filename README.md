# 📊 StudentLens — Student Performance Analyzer

A **Data Visualization + LLM** project built with Python, Matplotlib, Seaborn, and Claude AI on Streamlit.

## 🗂 Project Structure
```
student-performance-analyzer/
├── student_performance_dataset.csv          # Raw data (120 students)
├── student_performance_cleaned.csv          # Cleaned data (output of commit 1)
├── commit1_data_cleaning.py                 # Data cleaning & validation
├── commit2_subject_scores.py                # Subject score bar + box plots
├── commit3_grade_distribution.py            # Grade donut, bar, attendance bands
├── commit4_correlation_analysis.py          # Heatmap + scatter plots
├── commit5_attendance_studyhours.py         # Deep dive attendance & study hours
├── commit6_subject_comparison.py            # Radar chart + violin per grade
├── commit7_top_bottom_students.py           # Top 10 vs Bottom 10 analysis
├── commit8_llm_insights.py                  # Claude API integration module
├── commit9_streamlit_charts.py              # Streamlit dashboard — all charts
├── commit10_streamlit_llm.py                # Full app: charts + LLM insights
├── requirements.txt
└── plots/                                   # All saved chart images
```

## 📦 Installation
```bash
pip install -r requirements.txt
```

## 🔑 Set API Key
```bash
export ANTHROPIC_API_KEY="your-api-key-here"
```

## 🚀 Run the Final Dashboard
```bash
streamlit run commit10_streamlit_llm.py
```

## 🔢 Commit Breakdown

| # | File | What it adds |
|---|------|-------------|
| 1 | `commit1_data_cleaning.py` | Fix NaN, negative study hours, cap attendance |
| 2 | `commit2_subject_scores.py` | Average bar chart + box plot per subject |
| 3 | `commit3_grade_distribution.py` | Donut, count bar, attendance-band stacked bar |
| 4 | `commit4_correlation_analysis.py` | Heatmap + scatter: study hrs & attendance vs score |
| 5 | `commit5_attendance_studyhours.py` | Histograms, bubble chart, grouped bar per grade |
| 6 | `commit6_subject_comparison.py` | Radar chart + violin plot per subject & grade |
| 7 | `commit7_top_bottom_students.py` | Top 10 vs Bottom 10 comparison |
| 8 | `commit8_llm_insights.py` | Claude API module — 4 insight types |
| 9 | `commit9_streamlit_charts.py` | Streamlit app — full visualization dashboard |
| 10 | `commit10_streamlit_llm.py` | Streamlit app — charts + live AI insights |

## 📌 Dataset Features
| Column | Description |
|--------|-------------|
| Student_ID | Unique identifier |
| Math, Physics, Chemistry, English, Computer_Science | Subject scores (0–100) |
| Attendance_Percent | Class attendance % |
| Study_Hours_Per_Day | Daily study hours |
| Average_Marks | Overall average |
| Final_Grade | A / B / C |
