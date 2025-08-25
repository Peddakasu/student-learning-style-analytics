# Student Learning Styles & Academic Performance — Structured Data Analytics Project

This repository contains a full, **structured data analytics** workflow analyzing how student learning styles and behaviors relate to academic performance, plus an interactive **Power BI dashboard**.

> **Files included**: a clean CSV dataset, the full Jupyter Notebook, and a Power BI `.pbix` report.

---

## 🔍 Project Overview

- **Goal**: Explore patterns between learning styles/behaviors and outcomes (e.g., *Exam Score (%), Attendance Rate (%)*), and surface insights for educators and students.
- **Assets**:
  - `notebooks/DataAnalytics_P1.ipynb` — end‑to‑end analysis (EDA → preprocessing → visuals → insights).
  - `data/raw/student_learningstyle_and_performance_dataset.csv` — dataset used in the analysis.
  - `powerbi/Student Performance Learning Style Dashboard.pbix` — interactive dashboard.
- **Tech**: Python (**pandas**, **matplotlib**, **seaborn**, **plotly**, **scikit‑learn**), Power BI.

---

## 🗂️ Dataset

- **File**: `data/raw/student_learningstyle_and_performance_dataset.csv`
- **Shape**: **10000 rows × 15 columns**
- **Sample columns**: Student_ID, Age, Gender, Study_Hours_per_Week, Preferred_Learning_Style, Online_Courses_Completed, Participation_in_Discussions, Assignment_Completion_Rate (%) …
- **Target/Key metrics**: *Exam_Score (%), Attendance_Rate (%)* (see notebook for full details).

> The notebook documents assumptions, cleaning steps, and feature descriptions.

---

## 📒 Notebook Highlights (`notebooks/DataAnalytics_P1.ipynb`)

- Data validation and type checks
- Missing value handling and basic cleaning
- Univariate & bivariate EDA (distributions, relationships)
- Visualizations with matplotlib / seaborn / plotly
- Preprocessing with `sklearn.preprocessing` (e.g., encoding/scaling where needed)
- Insight summaries that connect behaviors to performance

> If you extended this with modeling or segmentation, add a short subsection here (e.g., *KMeans clustering for learner personas*).

---

## 📊 Power BI Dashboard (`powerbi/*.pbix`)

- Overview of key KPIs (Exam Score, Attendance, Assignment Completion)
- Slicers for **Preferred Learning Style**, **Gender**, **Study Hours**, etc.
- Drill‑downs to compare cohorts and behaviors

> Add screenshots in `reports/figures/` and reference them here.

---

## 🚀 Quickstart

### 1) Clone & set up environment

```bash
git clone <your-repo-url>.git
cd student-learning-style-analytics

# (Recommended) create a virtual environment
python -m venv .venv
# Windows: .venv\Scripts\activate
# macOS/Linux: source .venv/bin/activate

pip install -r requirements.txt
```

### 2) Run the notebook

```bash
jupyter notebook notebooks/DataAnalytics_P1.ipynb
# or: jupyter lab
```

### 3) Open the Power BI report

Open `powerbi/Student Performance Learning Style Dashboard.pbix` in **Power BI Desktop**.

---

## 🧱 Repository Structure

```
student-learning-style-analytics/
├─ data/
│  └─ raw/
│     └─ student_learningstyle_and_performance_dataset.csv
├─ notebooks/
│  └─ DataAnalytics_P1.ipynb
├─ powerbi/
│  └─ Student Performance Learning Style Dashboard.pbix
├─ reports/
│  └─ figures/            # (Add PNGs of charts/PBI screenshots here)
├─ src/                   # (Optional: helper modules, if any)
├─ docs/                  # (Optional: extra docs)
├─ requirements.txt
├─ .gitignore
├─ .gitattributes         # tracks .pbix with Git LFS
└─ README.md
```

---

## 📦 Managing Large Files (Power BI) with Git LFS

Power BI `.pbix` files can be big. To track them reliably:

```bash
# Install Git LFS once on your machine
git lfs install

# Ensure .pbix files are tracked with LFS (this repo already includes .gitattributes)
git lfs track "*.pbix"

# Verify and commit
git add .gitattributes
git add powerbi/*.pbix
git commit -m "Track Power BI report with Git LFS"
```

---

## ✍️ How to Cite on a Resume / Portfolio

- **Title**: *Student Learning Styles & Academic Performance — Data Analytics Project*
- **Highlights**: Performed EDA, built visuals, and created a Power BI dashboard to explore how learning behaviors correlate with performance on a 10,000‑row dataset.
- **Stack**: Python (pandas, plotly, seaborn, scikit‑learn), Power BI.
- **Link**: GitHub repository (and optional dashboard screenshots).

---

## 🧰 Requirements

See [`requirements.txt`](requirements.txt). Includes: `pandas`, `matplotlib`, `seaborn`, `plotly`, `scikit-learn`, and `mysql-connector-python` (for MySQL connectivity used in the notebook).

---

## 📄 License

Choose a license (e.g., MIT) and add a `LICENSE` file if you plan to share/reuse this work.
