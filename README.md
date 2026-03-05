# 📊 Dynamic Regional Sales Overview Dashboard | Power BI

## 📝 Project Overview
This project features an end-to-end, dynamic Power BI dashboard designed to track key business metrics—**Sales, Profit, and Quantity**—across multiple geographic regions. Built for higher management and regional stakeholders, the dashboard provides a high-level summary alongside granular, state-level insights to analyze performance trends, identify profitable regions, and compare year-over-year (YoY) growth.

## ✨ Key Features & Technical Highlights

* **Dynamic Metric Selection:** Implemented DAX parameters allowing users to seamlessly toggle the entire dashboard's context between Sales, Profit, and Quantity without duplicating visuals.
* **Advanced Time-Intelligence DAX:** * Custom DAX calculations to dynamically retrieve Current Year (CY) and Previous Year (PY) data based on user filter selections.
  * Robust error handling for historical data (e.g., dynamically displaying "No Data" when selecting the earliest available year to prevent blank visual errors).
* **Monthly Trend Sparklines:** Custom-built bar chart sparklines detailing monthly performance per region, enhanced with dynamic average lines to instantly spot above/below-average months.
* **Geospatial & Top/Bottom Analysis:** * A dynamically scaling Bubble Map chart visualizing state-wise performance.
  * Stacked Bar Charts to easily rank top-performing and underperforming states.
* **Comprehensive Financial Matrix (Grid View):** A detailed grid displaying CY metrics, PY metrics, and YoY % Change.
* **Conditional Formatting:** Utilized DAX `UNICHAR()` functions to integrate positive/negative directional arrows (▲/▼) and data bars directly into the matrix for intuitive visual cues.

## 🛠️ Tech Stack & Concepts Applied
* **Tool:** Power BI Desktop
* **Languages:** DAX (Data Analysis Expressions)
* **Data Modeling:** Designed a Star Schema integrating a central Sales Fact table with a custom-built Calendar/Date Dimension table (1-to-Many relationship).
* **Techniques:** Parameter Fields, Custom Variables in DAX, Data Transformation, UI/UX Layouting.

## 📸 Dashboard Preview
<img width="1328" height="742" alt="image" src="https://github.com/user-attachments/assets/c768058d-c52d-4479-bf25-20efd8df7975" />
<img width="1321" height="743" alt="image" src="https://github.com/user-attachments/assets/e585d910-e160-4289-8cae-419e1c898b66" />
<img width="1320" height="747" alt="image" src="https://github.com/user-attachments/assets/f49b0a94-0dd2-491d-99d0-bedfd82da971" />

## 📂 Repository Structure
* `Sales_Overview_Dashboard.pbix`: The complete Power BI project file containing the data model, DAX measures, and visual reports.
* `Dataset/`: Folder containing the raw sales data CSV/Excel file used for this analysis.
* `Background_Design/`: UI/UX layout assets or images used for the dashboard canvas background.

## 🚀 How to Open and Use
1. Download and install [Power BI Desktop](https://powerbi.microsoft.com/desktop/).
2. Clone or download this repository.
3. Open the `Sales_Overview_Dashboard.pbix` file.
4. Interact with the **Year Filter** and **Metric Slicer (Sales, Profit, Quantity)** on the top left to see the entire dashboard dynamically update.

---
**Author:** Shravan Mandal
