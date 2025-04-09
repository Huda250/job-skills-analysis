# Job Skills Analysis from Job Postings

## Overview
This project analyzes job postings data to identify the most in-demand technical and soft skills sought by employers. The analysis was based on a dataset containing job descriptions and listed skills, aiming to uncover patterns in skill requirements.

## Dataset
- File: `postings.csv`  
- Contains job posting data including columns like `first_seen`, `search_city`, `job_link`, `summary`, and `skills`.  
- Source: Provided via public dataset (original Kaggle link is no longer available).

## Tools Used
- Python
- Pandas
- Matplotlib
- Jupyter Notebook

## Key Steps
- Loaded and explored the dataset using Jupyter Notebook.
- Checked for and handled missing values (primarily in the `summary` and `skills` columns).
- Cleaned and standardized the `skills` column by removing null entries, trimming whitespace, and fixing case inconsistencies.
- Visualized the top 10 most frequent skills.
- Manually selected common technical and cognitive skills for a comparative bar chart.
- Noted data quality concerns due to free-text skill entry variability.

## Visualizations

### Top 10 Most In-Demand Skills
Displays the most frequently mentioned skills across all job postings after cleaning.

### Technical vs Cognitive Skills Comparison
Manually selected top skills grouped by category to explore employer emphasis on different skill types.

> *Note: The comparison is based on a manual selection from the top 30 skills, and not a fully automated grouping. Categorization was based on domain knowledge and the context of job postings.*

## Key Insights
- The top skills include Data Analysis, SQL, Communication, Project Management, and Excel.
- Case sensitivity and variations in spelling/phrasing significantly influenced the results.
- After standardizing cases (e.g., “analysis” vs “Analysis”), the top skills list changed noticeably.
- Soft skills like communication and teamwork were consistently present, alongside technical tools like Tableau and Excel.

## Limitations
- The `skills` data was entered as free text, leading to many unique but redundant entries (~46,000+ skill variants).
- Manual cleanup helped reduce duplication but could not catch all variations (e.g., "Microsoft Office Suite" vs. "Word/PowerPoint").
- Grouped plots were created from selected terms, not auto-categorized clusters.

## Future Work
- Apply NLP techniques or fuzzy matching to better consolidate similar skills.
- Categorize top 100+ skills programmatically by domain.
- Create an interactive dashboard for dynamic skill filtering and exploration.
