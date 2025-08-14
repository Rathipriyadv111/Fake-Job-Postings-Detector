# 🕵️ Fake Job Postings Detector

**Author:** Rathi Priya  
**Project:** Machine Learning-based Fake Job Posting Detection System

## 📋 Project Overview

This project analyzes job posting data to detect fraudulent job advertisements using data science and machine learning techniques. The system performs exploratory data analysis, handles missing values intelligently, and provides insights into patterns that distinguish fake job postings from legitimate ones.

## 🎯 Key Features

- **Data Analysis**: Comprehensive exploratory data analysis of job posting features
- **Missing Value Analysis**: Advanced techniques to understand missing data patterns
- **Visualization**: Interactive plots showing relationships between features and fraudulent status
- **Data Preprocessing**: Automated data cleaning and preparation pipeline
- **Fraud Detection**: Binary classification to identify fake job postings

## 📊 Dataset Information

- **Size**: 17,880 job postings with 18 features
- **Target Variable**: `fraudulent` (0 = Legitimate, 1 = Fake)
- **Class Distribution**: ~4.8% fraudulent postings (imbalanced dataset)
- **Features Include**: Job title, location, company profile, salary range, requirements, benefits, etc.

## 🛠️ Technologies Used

- **Python 3.8+**
- **Data Analysis**: Pandas, NumPy
- **Visualization**: Matplotlib, Seaborn
- **Machine Learning**: Scikit-learn (for future enhancements)
- **Text Processing**: NLTK, TextBlob (optional)

## 🚀 Quick Start

### Prerequisites
- Python 3.8 or higher
- pip package manager

### Installation & Setup

1. **Clone or download this repository**
```bash
git clone <repository-url>
cd Fake-Job-Postings-Detector-main
```

2. **Create virtual environment (Recommended)**
```bash
python -m venv fake_job_env

# Activate virtual environment
# Windows:
fake_job_env\Scripts\activate
# macOS/Linux:
source fake_job_env/bin/activate
```

3. **Install required packages**
```bash
pip install pandas numpy seaborn matplotlib
```

4. **Verify installation**
```bash
python -c "import pandas, numpy, seaborn, matplotlib; print('All packages installed successfully!')"
```

5. **Run the analysis**
```bash
python app.py
```

### Optional Advanced Packages
For extended functionality, install additional packages:
```bash
pip install scikit-learn wordcloud nltk textblob plotly xgboost lightgbm imbalanced-learn
```

## 📁 Project Structure

```
Fake-Job-Postings-Detector-main/
├── app.py                    # Main analysis script
├── fake_job_postings.csv     # Dataset file
├── README.md                 # Project documentation
└── requirements.txt          # Dependencies (if needed)
```

## 🔍 What the Script Does

1. **Data Loading & Exploration**
   - Loads the job postings dataset
   - Displays basic dataset information (shape, columns, data types)
   - Shows summary statistics and missing value percentages

2. **Data Cleaning**
   - Identifies and removes duplicate entries
   - Creates missing value indicator flags
   - Preserves original data integrity

3. **Missing Value Analysis**
   - Analyzes patterns in missing data
   - Visualizes missing value rates by fraudulent status
   - Helps determine if missing values are informative features

4. **Visualization**
   - Generates bar plots showing missing value patterns
   - Compares legitimate vs fraudulent job postings
   - Provides insights for feature engineering

## 📈 Expected Output

When you run the script, you'll see:
- Dataset overview and statistics
- Missing value percentages for each column
- Number of duplicate rows (if any)
- Interactive visualization showing missing value patterns by fraudulent status

## 🔧 Troubleshooting

| Issue | Solution |
|-------|----------|
| `python command not found` | Try `python3` instead of `python` |
| `pip not found` | Use `python -m pip install package_name` |
| `File not found error` | Ensure `fake_job_postings.csv` is in the same folder |
| `Permission denied` | Run terminal as administrator (Windows) |
| `Module not found` | Activate virtual environment and reinstall packages |

## 🎯 Future Enhancements

- [ ] Implement machine learning models (Random Forest, XGBoost, Neural Networks)
- [ ] Add text analysis for job descriptions and requirements
- [ ] Create interactive dashboard using Plotly/Streamlit
- [ ] Implement SMOTE for handling class imbalance
- [ ] Add model evaluation metrics and cross-validation
- [ ] Deploy as web application

## 👨‍💻 Author Information

**Rathi Priya**
- Data Science & Machine Learning Enthusiast
- Focus: Fraud Detection and Pattern Analysis

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the issues page.

---

**Note**: Make sure you have the `fake_job_postings.csv` dataset file in the same directory as `app.py` before running the script.