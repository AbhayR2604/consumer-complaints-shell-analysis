# Consumer Complaints Data Wrangling Using Shell Commands

## Project Overview

This project demonstrates shell-based data wrangling and exploratory analysis on a consumer complaints dataset. The analysis uses Unix command-line tools such as `awk`, `cut`, `sort`, `uniq`, `wc`, and `head` to clean complaint records, validate IDs, extract dates, analyse product categories, and identify text patterns in complaint narratives.

The project focuses on using command-line techniques to inspect, filter, and summarise structured complaint data efficiently.

## Objectives

The analysis covers the following tasks:

1. Identify the date range of complaint records.
2. Validate Complaint IDs and clean date values.
3. Remove invalid records and create a filtered complaints dataset.
4. Search complaint narratives for specific financial product terms.
5. Analyse product category frequency.
6. Identify fraud-related credit card complaints.
7. Identify complaints involving long wait times.

## Tools and Technologies

- Unix Shell Commands
- `awk`
- `cut`
- `sort`
- `uniq`
- `wc`
- `head`
- Regular Expressions
- CSV File Processing

## Key Analysis Steps

### 1. Date Range Extraction

The `Date_received` column was processed to identify the earliest and latest complaint dates in the dataset. Time values were removed to focus only on the date component.

### 2. Complaint ID Validation

Complaint IDs were checked using regular expressions to ensure that each ID followed the expected seven-digit numeric format. Invalid records were counted and excluded from further analysis.

### 3. Data Cleaning

A cleaned version of the dataset was created by:

- Removing records with invalid Complaint IDs
- Removing time values from the `Date_received` column
- Saving the cleaned output as `filtered_complaints.csv`

### 4. Product Category Analysis

The product column was analysed to identify:

- The number of unique product categories
- The top five most frequent product categories based on complaint narratives

### 5. Text Pattern Matching

Complaint narratives were searched using case-insensitive pattern matching to identify:

- Fraud-related credit card complaints
- Complaints involving long wait times and time-based expressions

## Skills Demonstrated

- Shell scripting
- Data cleaning
- Regular expressions
- Text pattern matching
- CSV filtering
- Frequency analysis
- Command-line data exploration
- Basic text analysis

## Files in This Repository

```text
consumer-complaints-shell-analysis/
│
├── README.md
└── consumer-complaints-shell-analysis.docx
