# Julius AI — Complete Step-by-Step Guide

> **Julius AI** is an AI-powered data analysis platform that lets you analyze spreadsheets, CSVs, PDFs, and databases using plain English — no coding required.

---

## Table of Contents

1. [What is Julius AI?](#1-what-is-julius-ai)
2. [Getting Started — Create an Account](#2-getting-started--create-an-account)
3. [Uploading Your Data](#3-uploading-your-data)
4. [Connecting Data Sources](#4-connecting-data-sources)
5. [Analyzing Data with Natural Language](#5-analyzing-data-with-natural-language)
6. [Creating Visualizations](#6-creating-visualizations)
7. [Exploratory Data Analysis (EDA)](#7-exploratory-data-analysis-eda)
8. [Using Notebooks (Reusable Templates)](#8-using-notebooks-reusable-templates)
9. [Scheduling Automated Reports](#9-scheduling-automated-reports)
10. [Sharing & Exporting Results](#10-sharing--exporting-results)
11. [Plans & Pricing Overview](#11-plans--pricing-overview)
12. [Tips & Best Practices](#12-tips--best-practices)
13. [Useful Prompt Examples](#13-useful-prompt-examples)

---

## 1. What is Julius AI?

Julius AI is an intelligent data analyst tool that interprets, analyzes, and visualizes complex data in an intuitive, user-friendly manner. It makes data analysis accessible and actionable — even for people who are not data scientists.

**Key capabilities:**
- Chat with your data using plain English
- Generate charts, forecasts, and insights automatically
- Supports Excel, CSV, PDF, Google Sheets, images, and databases
- No coding knowledge required

---

## 2. Getting Started — Create an Account

1. Go to [https://julius.ai](https://julius.ai)
2. Click **Get Started** or **Sign Up**
3. Register with your Google account or email address
4. Confirm your email if prompted
5. You'll land on a clean **workspace/chat page** — ready to analyze

> 💡 A **free plan** is available that includes **15 messages per month**, great for exploring core features before committing to a paid plan.

---

## 3. Uploading Your Data

1. On the Chat page, click the **paperclip (📎) button** in the message input area
2. Select your file from your device
3. Julius will automatically ingest and parse the file

**Supported file formats include:**

| Format | Examples |
|--------|----------|
| Spreadsheets | `.xlsx`, `.xls`, `.csv` |
| Documents | `.pdf`, `.docx`, `.txt` |
| Google Sheets | Link directly |
| Images | `.jpeg`, `.png` |
| Databases | BigQuery, PostgreSQL, and more |

> 💡 **Multi-tab spreadsheets** are fully supported. Refer to individual tab names in your prompts and Julius will analyze them separately.

---

## 4. Connecting Data Sources

Julius supports **live data connections** so you don't need to manually re-upload files.

### Steps to connect a data source:
1. Go to the **Files** page (left sidebar)
2. Click **Add Data Source** or **Link Source**
3. Choose from available integrations:
   - Google Sheets
   - Google Ads
   - BigQuery
   - PostgreSQL / other databases
4. Authenticate and grant access
5. Your data is now live — Julius pulls from it in real time

> 💡 You can also **@ mention specific tables or columns** in chat so Julius knows exactly what data to analyze without back-and-forth clarification.

---

## 5. Analyzing Data with Natural Language

Once your data is uploaded or connected:

1. Go to the **Chat** page
2. Type your question or instruction in plain English in the message box
3. Press **Enter** or click **Send**
4. Julius interprets your intent, executes the analysis, and returns results

**Example prompts to get started:**
```
Show me the sales trends for the last quarter.
What is the average revenue per customer?
Which product category has the highest return rate?
Summarize the key statistics of this dataset.
```

Julius understands follow-up questions, so you can refine your analysis conversationally.

---

## 6. Creating Visualizations

Julius generates charts and graphs automatically — no separate tools needed.

### How to request a visualization:
1. Type a prompt asking for a chart or graph, e.g.:
   ```
   Create a bar chart of monthly revenue by region.
   Show a pie chart of customer segments by revenue.
   Plot a histogram of delivery times.
   ```
2. Julius generates the visualization inline in the chat
3. You can ask follow-up questions to modify it:
   ```
   Change the color scheme to blue tones.
   Add a trendline to this chart.
   Break this down by year instead of month.
   ```

**Visualization types Julius supports:**
- Bar charts & Histograms
- Line charts & Trend plots
- Pie charts & Donut charts
- Box plots
- Scatter plots
- Dashboards

---

## 7. Exploratory Data Analysis (EDA)

Julius makes it easy to perform a full EDA on any dataset.

### Step-by-step EDA workflow:

**Step 1 — Get summary statistics**
```
Give me a statistical summary of this dataset.
```
Julius returns count, mean, standard deviation, min/max, and interquartile ranges for each column.

**Step 2 — Check for missing values**
```
Check the columns for missing data please.
```
Julius identifies all columns with null or missing values and suggests how to handle them.

**Step 3 — Explore distributions**
```
Plot the distribution of the Age column.
```

**Step 4 — Find correlations**
```
What variables are most correlated with sales?
Show a correlation heatmap.
```

**Step 5 — Detect outliers**
```
Are there any outliers in the Revenue column?
```

> 💡 If you're unsure about a statistic, just ask Julius to explain it in plain English — it's one of the key benefits of using an AI-powered tool.

---

## 8. Using Notebooks (Reusable Templates)

Julius **Notebooks** are reusable analysis templates you can build once and run again on new data.

1. Complete an analysis in Chat
2. Click **Save as Notebook** (or find the option in the menu)
3. Name your notebook (e.g., "Monthly Revenue Report")
4. To reuse it: open the Notebooks section, select your template, upload new data, and run

This is ideal for recurring reports like weekly revenue summaries or monthly KPI tracking.

---

## 9. Scheduling Automated Reports

Julius lets you automate recurring analyses and have them delivered to you automatically.

### Steps to schedule a report:
1. Set up the analysis you want to automate in Chat
2. Click **Schedule** or access scheduling through the Reports section
3. Set the frequency: **daily**, **weekly**, or **monthly**
4. Choose delivery method: **email** or **Slack**
5. Confirm and save the schedule

**Example use cases:**
- Weekly revenue summary delivered every Monday morning
- Monthly delivery time percentile report sent to Slack
- Daily Google Ads performance digest via email

---

## 10. Sharing & Exporting Results

### Export as PDF Report:
1. After completing your analysis in Chat
2. Click **Create Report** (located near the top or in the chat options)
3. Julius pulls key takeaways and visualizations from your chat
4. Download as a **PDF** or share a link with your team

> 💡 One-click sharing turns any thread of analysis into a clean, shareable report — no extra formatting needed.

### Write results back to Google Sheets:
1. Connect your Google Sheets data source (see Step 4)
2. After analysis, prompt Julius:
   ```
   Write the scores/results back to my Google Sheet.
   ```
3. Julius updates the sheet automatically

---

## 11. Plans & Pricing Overview

| Plan | Messages/Month | Best For |
|------|---------------|----------|
| **Free** | 15 messages | Exploring the platform |
| **Pro** | Unlimited | Regular data analysis work |
| **Team/Enterprise** | Custom | Business teams and organizations |

> ✅ The **Pro plan** (monthly or annual) is recommended if you do regular or automated data analysis.
> Always check [julius.ai](https://julius.ai) for the latest pricing.

---

## 12. Tips & Best Practices

- **Be specific in your prompts** — Instead of "analyze my data", say "show me monthly revenue trends for 2024."
- **Use @ mentions** — Tag specific tables or columns to get accurate answers faster.
- **Start broad, then refine** — Ask for a summary first, then drill down into specifics.
- **Ask for explanations** — If you don't understand a result, ask "What does this mean?" and Julius will explain.
- **Use Notebooks for recurring tasks** — Save time by templatizing repeated analyses.
- **Connect live sources** — Avoid stale data by linking Google Sheets or databases directly.
- **Review privacy policies** — Always check Julius's current privacy policy before uploading sensitive or confidential data.

---

## 13. Useful Prompt Examples

### Data Cleaning
```
Check for duplicate rows and remove them.
Fill missing values in the Age column with the median.
Rename column "cust_id" to "Customer ID".
```

### Analysis
```
What are the top 5 products by total sales?
Compare Q1 vs Q2 performance across all regions.
Show me the month-over-month growth rate.
Which customers have the highest lifetime value?
```

### Visualization
```
Create a line chart showing revenue growth over the last 12 months.
Build a dashboard showing KPIs: revenue, orders, and churn rate.
Plot a scatter chart of marketing spend vs. customer acquisition.
```

### Forecasting
```
Forecast next quarter's revenue based on current trends.
Predict monthly sales for the next 6 months.
```

---

## Resources

- 🌐 **Website:** [https://julius.ai](https://julius.ai)
- 📖 **Official Guides:** [https://julius.ai/guides](https://julius.ai/guides)
- 💬 **LinkedIn:** [Julius AI on LinkedIn](https://www.linkedin.com/company/julius-ai)

---

*Last updated: May 2026*
