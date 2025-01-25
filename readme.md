# RFM Analysis on Students' Union Purchases

## Project Overview
This project applies algorithms and data structures to analyze a dataset of purchase history from a Students' Union (SU). Using the RFM (Recency, Frequency, Monetary) model, the project identifies and ranks students based on their purchase behavior. The analysis leverages efficient sorting, searching, and ranking algorithms implemented in Python.

## Objectives
The primary objectives of the project were:
1. Calculate RFM scores to classify students based on their purchase history.
2. Explore and visualize the dataset to extract meaningful insights.
3. Implement efficient algorithms for sorting (Merge Sort) and searching.
4. Correlate traditional RFM scores with a nested RFM model (RFM’).
5. Deliver a well-documented and executable Jupyter Notebook.

## Problem Statement
Understanding customer behavior is essential for effective marketing and engagement strategies. The Students' Union lacked a systematic way to identify their most valuable customers. This project aims to address this gap by ranking students based on their purchasing patterns using RFM analysis.

## Methodology
### Dataset
The dataset includes:
- **Name**: Student's name (unique identifier for analysis).
- **Date**: Purchase date as a tuple (DD, MM, YYYY).
- **Item**: Name of the purchased item.
- **Unit Price**: Price per unit of the item in Euros.
- **Quantity**: Number of items purchased.

### Steps
1. **Data Exploration and Preparation**:
   - Calculated recency (days since last purchase), frequency (total purchases), and monetary value (total spent) for each student.
   - Plotted histograms for recency, frequency, and monetary value using Matplotlib.

2. **Sorting**:
   - Implemented **Merge Sort** to rank students by recency, frequency, and monetary value.
   - Assigned scores (1 to 3) to each student based on sorted results.

3. **RFM Scoring**:
   - **First RFM Score**:
     - Assigned independent recency, frequency, and monetary scores.
     - Combined scores to rank students.
   - **Second RFM Score (Nested)**:
     - Nested ranking within recency buckets, followed by frequency and monetary value.
     - Correlated RFM and RFM’ scores using Spearman’s rank correlation.

4. **Searching**:
   - Used linear and binary search to find RFM scores of specific students.
   - Measured time complexity using Python's `timeit` module.

### Deliverables
- A Jupyter Notebook with:
  - Clear, commented Python code.
  - Visualizations and outputs for each task.
  - Results of sorting, RFM analysis, and correlation tests.

## Key Insights
1. Students with high RFM scores (e.g., 333) represent the most valuable customers for the SU.
2. Correlation between RFM and RFM’ scores provided additional insights into customer segmentation.
3. Binary search significantly reduced search time compared to linear search, demonstrating the advantages of sorting.

## Conclusion
This project successfully implemented an RFM model to rank and identify valuable customers. Efficient algorithms, including Merge Sort for sorting, and data visualization provided actionable insights for targeted marketing and engagement strategies. The analysis showcases the power of algorithms and data structures in real-world applications.
