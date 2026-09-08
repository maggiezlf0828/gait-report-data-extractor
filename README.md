# PDF Report Data Extractor

A Python-based data extraction tool that reads semi-structured PDF reports, extracts selected measurements using regular expressions, organizes the results with pandas, and exports the structured data to Excel.

## Overview

This project was created to automate the process of extracting numerical measurements from PDF reports.

The script uses `pdfplumber` to read PDF text and extracts several types of information, including:

- Mean and standard deviation values in formats such as `64.0 ± 1.6`
- Left-side (`L`) and right-side (`R`) measurements
- Selected force-related metrics
- Maximum gait line velocity
- Structured Excel output

The generated Excel file automatically uses the same base filename as the original PDF.

For example:

```text
58bpmDT.pdf
