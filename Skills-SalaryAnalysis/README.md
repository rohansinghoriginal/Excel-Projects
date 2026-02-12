# Data Market Analysis: Strategic Insights into Salaries & Skills

## 🎯 Project Overview
In a competitive landscape, I engineered an end-to-end analysis of the 2023 data science job market. The goal was to identify "high-leverage" skills—the specific technical competencies that correlate with premium compensation and regional demand.

### 💡 Key Business Questions
* **Compensation Drivers:** Does skill diversification directly influence salary scaling?
* **Geographic Arbitrage:** How do compensation benchmarks fluctuate across global regions?
* **ROI of Learning:** What is the financial valuation of the top 10 most in-demand skills?

---

## 🛠️ Technical Stack (Advanced Excel BI)
To ensure scalability, I utilized Excel’s professional BI suite rather than basic spreadsheet functions:
* **Power Query:** Executed complex ETL processes to sanitize and structure raw market data.
* **Power Pivot & DAX:** Built a relational data model to calculate sophisticated measures.
* **Pivot Charts:** Developed dynamic visualizations to translate raw data into career intelligence.

---

## 1️⃣ Process Methodology: ETL & Data Architecture

### 🔄 Extraction & Transformation
Using **Power Query**, I transformed a messy, multi-variable dataset into a structured analytical engine by:
![2_Project_Analysis_Screenshot1.png](/Excel/Images/2_Project_Analysis_Screenshot1.png)![2_Project_Analysis_Screenshot2.png](/Excel/Images/2_Project_Analysis_Screenshot2.png)
* **Normalization:** Split data into two optimized tables (**Job Intelligence** and **Skills Taxonomy**) to minimize redundancy.
![2_Project_Analysis_Screenshot3.png](/Excel/Images/2_Project_Analysis_Screenshot3.png)![2_Project_Analysis_Screenshot4.png](/Excel/Images/2_Project_Analysis_Screenshot4.png)
* **Data Scrubbing:** Standardized data types, removed outliers, and performed string manipulation to ensure a "source of truth."

 ![2_Project_Analysis_Chart1.png](/Excel/Images/2_Project_Analysis_Chart1.png)


### 🔗 Relational Modeling
I established a **1-to-Many relationship** between the tables using the `job_id`. This architecture allows for seamless updates as new 2024/2025 market data becomes available without breaking existing reports.

---

## 2️⃣ Geographic & Skill-Based Analysis

### 🧮 Advanced Modeling with DAX
I moved beyond basic averages by using DAX to isolate specific market segments. 
**Example Measure:**
$$Median\ Salary\ US = CALCULATE(MEDIAN(data\_jobs[salary]), data\_jobs[country] = "United States")$$

### 📊 Key Insights
* **The "Complexity Premium":** There is a sharp positive correlation between technical skill density and median salary. High-impact roles (Senior Data Engineers/Scientists) exhibit the steepest salary scaling as skill count increases.
* **The "US Tech Premium":** While global demand is high, a pronounced salary gap exists between US and international roles, driven by the density of high-growth tech hubs.
![2_Project_Analysis_Chart2.png](/Excel/Images/2_Project_Analysis_Chart2.png)


---

## 3️⃣ Mapping the Technical Landscape

### 💡 Demand vs. Reward
By engineering a **Dual-Axis Correlation Analysis**, I mapped the intersection of market frequency (how often a skill is requested) and financial reward.
![2_Project_Analysis_Chart3.png](/Excel/Images/2_Project_Analysis_Chart3.png)
* **The "Golden Stack":** **SQL** and **Python** remain the undisputed foundations of the ecosystem.
* **Cloud Transformation:** The heavy presence of **AWS** and **Azure** in high-pay brackets signals a mandatory shift toward cloud-native data architectures.
![2_Project_Analysis_Chart4.png](/Excel/Images/2_Project_Analysis_Chart4.png)
* **The Commodity Gap:** Administrative tools (Word/PowerPoint) show the lowest correlation with salary growth, confirming that market value is driven by technical specialization.

---

## 🏁 Conclusion
This analysis serves as a roadmap for career optimization. The findings prove that **technical depth in SQL, Python, and Cloud technologies** provides the greatest statistical probability of a salary increase. This project demonstrates my ability to take complex, real-world data and extract the strategic intelligence required for high-level decision-making.
