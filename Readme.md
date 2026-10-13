# EduSpace — Campus Facility Utilization Analysis and Optimization

**Course:** U23AD491 – Data Science  
**Assessment:** DS Sprint – Skill-Based Assessment 2  
**Domain:** Campus Facility Management and Data Analytics

---

## 1. Problem Statement

Educational institutions manage various facilities, including classrooms, laboratories, libraries, seminar halls, and common spaces. However, limited visibility into booking schedules, actual occupancy, peak usage periods, and maintenance downtime makes it difficult to allocate resources efficiently.

EduSpace aims to analyze campus facility utilization using data analytics, exploratory data analysis (EDA), feature engineering, Python, and Microsoft Excel.

The project integrates booking records, occupancy readings, facility information, academic calendars, and maintenance records to identify underutilized facilities, overcrowding, peak usage periods, and maintenance-related losses.

The primary goal is to provide data-driven insights that help campus management improve facility allocation, optimize scheduling, reduce congestion, and make better resource-management decisions.

## 2. Business Context

EduSpace manages multiple campus facilities with different capacities, purposes, locations, and availability schedules.

Campus management needs to understand:

- Which facilities are used most frequently.
- When and where overcrowding occurs.
- Which facilities remain underutilized.
- How examinations and campus events influence usage.
- Which facilities lose availability due to maintenance.
- Whether facility capacity matches actual occupancy demand.

## 3. Business Question

**How are campus facilities used, and where can utilization be improved?**

The analysis will translate facility data into actionable business recommendations for better scheduling, capacity planning, and maintenance management.

## 4. Business Approach

The project follows a structured data analytics workflow:

1. **Data Acquisition:** Obtain suitable datasets for bookings, facilities, occupancy, calendar events, and maintenance.
2. **Data Understanding:** Examine dataset structures, column names, data types, record counts, and relationships.
3. **Data Quality Assessment:** Identify missing occupancy readings, duplicate bookings, inconsistent facility names, occupancy above capacity, and incomplete maintenance records.
4. **Data Preprocessing:** Clean, standardize, validate, and combine the datasets at an appropriate analysis level.
5. **Exploratory Data Analysis:** Examine utilization patterns, peak periods, facility usage, downtime, and exam-period differences.
6. **Feature Engineering:** Create variables such as utilization percentage, booking duration, time slots, day of the week, and exam-period indicators.
7. **Data Visualization:** Develop meaningful charts to communicate usage trends and operational issues.
8. **Excel Analysis:** Build formulas, Pivot Tables, Pivot Charts, and a management summary dashboard.
9. **Business Insights:** Convert analytical findings into practical recommendations.
10. **Presentation:** Present evidence-based findings, proposed actions, and expected operational benefits.

## 5. Dataset Description

The project uses five related datasets.

| Dataset | Key Fields | Purpose |
|---|---|---|
| `bookings.csv` | facility, date, start, end, purpose | Analyze booking frequency, duration, and scheduling |
| `facilities.csv` | facility, type, capacity, block | Understand facility characteristics and capacity |
| `occupancy.csv` | timestamp, facility, count | Measure actual recorded occupancy |
| `calendar.csv` | date, working day, event, exam period | Analyze academic schedules and event-related changes |
| `maintenance.csv` | facility, issue, downtime | Measure maintenance frequency and availability losses |

Data may be obtained from suitable public sources, institution-provided files, or clearly documented simulated records where real data is unavailable. Simulated data will not be presented as actual campus observations.

## 6. Assessment Workflow — Round by Round

### Round 1: Quiz — 20 Marks

**Objective:** Demonstrate foundational knowledge of data analytics and related tools.

**Activities:**
- Answer objective questions on data analytics and preprocessing.
- Revise exploratory data analysis and feature engineering.
- Practice Microsoft Excel formulas and statistical functions.
- Understand NumPy and Pandas operations.
- Review Matplotlib and Seaborn visualizations.

**Expected Deliverables:**
- Completed MCQ assessment.
- Quiz score sheet.

### Round 2: EDA and Feature Engineering — 30 Marks

**Objective:** Prepare reliable data and discover meaningful campus utilization patterns.

**Activities:**

**A. Load and Understand Data**
- Import the five CSV files using Pandas.
- Inspect dimensions, column names, data types, and sample records.
- Understand relationships between facilities, bookings, occupancy, calendar events, and maintenance.

**B. Data Quality Assessment**
- Identify and handle missing occupancy readings.
- Detect duplicate bookings.
- Standardize inconsistent facility names.
- Investigate occupancy values exceeding facility capacity.
- Identify incomplete maintenance records.
- Validate dates, times, durations, and unusual values.

**C. Data Cleaning and Integration**
- Clean and standardize individual datasets.
- Remove or resolve duplicates using appropriate business rules.
- Merge datasets using facility identifiers and relevant dates or timestamps.
- Avoid incorrect joins that duplicate occupancy readings or inflate utilization metrics.
- Prepare an analysis-ready dataset at a clearly defined time or booking level.

**D. Exploratory Data Analysis**
- Rank facilities by usage and occupancy.
- Identify peak days and time slots.
- Compare actual occupancy against capacity.
- Identify underutilized facilities.
- Compare usage during examination and non-examination periods.
- Analyze maintenance frequency and downtime.
- Explore relationships between booking schedules and actual occupancy.

**E. Feature Engineering**
- Calculate booking duration.
- Extract hour, day of week, month, and time slot.
- Calculate utilization percentage using occupancy and capacity.
- Create exam-period and working-day indicators.
- Derive peak-period and underutilization indicators using documented thresholds.
- Create suitable analytical features for further analysis.

**F. Feature Selection**
- Select relevant variables for utilization analysis.
- Remove redundant or irrelevant columns where appropriate.
- Use correlation analysis or other suitable selection techniques.
- Apply dimensionality reduction only if justified by the data and analytical objective.

**Expected Deliverables:**
- Cleaned and prepared datasets.
- Python EDA notebook.
- Data quality assessment.
- Meaningful visualizations.
- Engineered features.
- Selected analytical features.

### Round 3: Data Analysis Using Excel — 30 Marks

**Objective:** Communicate the findings through spreadsheet-based analysis and reporting.

**Activities:**

**A. Import and Organize Data**
- Import cleaned data into Microsoft Excel.
- Format dates, times, percentages, and numeric fields.
- Organize worksheets with clear names and headings.
- Convert appropriate ranges into Excel Tables.

**B. Apply Formulas and Statistical Functions**
- Use `SUM`, `AVERAGE`, `COUNTIF`, `SUMIF`, and `AVERAGEIF` where appropriate.
- Use conditional formulas to classify underused or high-utilization facilities.
- Calculate occupancy and utilization percentages.
- Calculate booking durations and downtime summaries.
- Apply suitable statistical functions to compare usage patterns.

**C. Create Pivot Tables and Pivot Charts**
- Summarize utilization by facility, type, block, and time slot.
- Compare examination and non-examination periods.
- Summarize maintenance incidents and downtime.
- Identify facilities with low usage and high demand.
- Create Pivot Charts to communicate the findings.

**D. Build the Summary Dashboard**
- Present key utilization indicators.
- Show the most-used and least-used facilities.
- Highlight peak occupancy periods.
- Display examination-period comparisons.
- Summarize maintenance-related availability losses.
- Compare capacity with observed occupancy.

**Expected Deliverables:**
- Organized Excel workbook.
- Formula-based calculations.
- Pivot Tables and Pivot Charts.
- Analytical charts.
- Summary dashboard containing important results.

### Round 4: Pitching Business Insights — 20 Marks

**Objective:** Present findings and recommend actions that improve campus facility utilization.

**Activities:**

**A. Identify Key Findings**
- Identify facilities with high and low utilization.
- Highlight recurring peak occupancy periods.
- Identify capacity mismatches and potential congestion.
- Explain changes during examination periods and campus events.
- Highlight facilities affected by frequent or prolonged maintenance.

**B. Support Findings with Evidence**
- Use calculated metrics, summary tables, and charts.
- Quantify differences between facilities and time periods.
- Distinguish observed patterns from possible explanations.
- Avoid unsupported claims about causes or expected savings.

**C. Recommend Business Actions**
- Reschedule activities to reduce peak-period congestion.
- Reallocate suitable bookings to underused facilities.
- Review capacity planning for high-demand rooms.
- Schedule preventive maintenance during lower-demand periods where feasible.
- Improve occupancy monitoring and booking data quality.
- Establish utilization indicators for ongoing facility management.

**D. Prepare the Business Pitch**
- Introduce the campus utilization problem.
- Explain the analytical approach.
- Present the most important findings.
- Describe their business impact.
- Recommend specific actions supported by evidence.
- Conclude with measurable indicators for monitoring improvement.

**Expected Deliverables:**
- Short presentation slides.
- Evidence-backed business insights.
- Data-driven recommendations.
- Clear verbal explanation of the analysis.

## 7. Key Business Metrics

The following metrics will be considered where the required data is available:

| Metric | Purpose |
|---|---|
| Booking count | Measure booking frequency |
| Total booked hours | Measure scheduled facility usage |
| Average occupancy | Measure typical observed demand |
| Peak occupancy | Identify periods of highest recorded demand |
| Utilization percentage | Compare occupancy against available capacity |
| Underutilization rate | Identify facilities with consistently low usage |
| Maintenance downtime | Measure availability lost to maintenance |
| Exam-period usage change | Compare usage during exams and other periods |
| Capacity exceedance count | Identify records requiring investigation |

**Important:** Occupancy-based utilization and booking-based utilization are different measures. The analysis will distinguish actual observed occupancy from scheduled bookings and will account for missing readings and facility availability when calculating appropriate metrics.

## 8. Proposed Solution

EduSpace will produce an integrated data analytics workflow that transforms raw campus facility records into reliable utilization metrics and actionable business insights.

The Python analysis will provide data cleaning, dataset integration, EDA, feature engineering, and visualizations. Microsoft Excel will provide accessible summaries, formulas, Pivot Tables, Pivot Charts, and a management dashboard. The final presentation will communicate the most important findings and recommend practical scheduling, capacity-planning, and maintenance improvements.

The project will focus on descriptive and diagnostic analytics rather than assuming that a machine-learning model is necessary. Advanced predictive methods may be considered only if the available data supports a meaningful business objective.

## 9. Final Project Deliverables

The completed project will contain:

1. **Cleaned Dataset:** Validated and integrated analytical data.
2. **Python Notebook:** Data loading, quality checks, preprocessing, EDA, visualizations, and feature engineering.
3. **Excel Workbook:** Formulas, statistics, Pivot Tables, Pivot Charts, and a summary dashboard.
4. **Business Presentation:** Key findings, evidence, recommendations, and expected operational benefits.
5. **Project Documentation:** Dataset sources, cleaning decisions, metric definitions, assumptions, and limitations.

## 10. Success Criteria

The project will be considered successful when it can:

- Reliably identify facility utilization patterns.
- Highlight peak periods and underused spaces.
- Compare observed occupancy with available capacity.
- Explain differences between examination and non-examination periods.
- Quantify maintenance downtime where records permit.
- Present clear, evidence-based recommendations.
- Deliver reproducible analysis through Python and understandable reporting through Excel.

The ultimate goal is to help EduSpace make better decisions about how campus facilities are scheduled, allocated, monitored, and maintained.