# Data-Cleaning-Entity-Matching
## Overview
This project demonstrates a data cleaning and entity matching workflow for identifying duplicate and existing healthcare practice records in the absence of a reliable primary key.

The problem is based on a real-world scenario involving inconsistent
manual data entry, duplicate entities, and conflicting records.

## Problem
- No unique identifier
- Inconsistent text formatting
- Duplicate practices and practitioners
- One-to-many relationships
- Excel-based matching producing unreliable results

## Solution
- Normalize all identifying fields
- Use composite matching across multiple attributes
- Apply fuzzy string matching for names and addresses
- Score matches instead of binary classification
- Categorize records as Existing, New, or Conflict

## Tools
- Python
- pandas
- difflib / RapidFuzz (optional)
- Excel (review output)

## Output
The workflow produces an Excel file containing:
- Match score
- Match classification (Existing / New / Conflict)
- Match explanation

The output is intended for business review and manual validation.

## Notes
All data used in this project is synthetic and does not contain
any real or sensitive information.
