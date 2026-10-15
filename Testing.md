# 🧪 Dream Car Finder — Testing Documentation

## 1. Overview

This document describes the functional testing performed on Dream Car Finder, a no-code AI chatbot built using Botpress. The testing focuses on car discovery, filtering, model comparison, missing information handling, and EMI calculations.

## 2. Testing Environment

- **Application:** Dream Car Finder
- **Platform:** Botpress
- **Data Source:** Uploaded car-company CSV datasets in the Botpress Knowledge Base
- **Testing Type:** Functional testing
- **Test Cases:** 6

## 3. Test Cases and Results

| Test ID | Test Scenario | Expected Result | Status |
|---|---|---|---|
| TC-01 | Find cars under ₹10 lakh | Return suitable cars within the specified budget | PASS |
| TC-02 | Filter cars by fuel type and seating capacity | Return cars matching the requested criteria | PASS |
| TC-03 | Compare two car models | Present a side-by-side comparison using available specifications | PASS |
| TC-04 | Request a car absent from the dataset | Avoid presenting unsupported vehicle details as verified facts | PASS |
| TC-05 | Check a car with a missing price | Clearly acknowledge unavailable price information | PASS |
| TC-06 | Verify EMI calculation | Calculate EMI using the specified interest rate and loan tenure | PASS |

## 4. Testing Approach

### Car Discovery and Filtering
Tested whether the chatbot could respond to budget-based searches and filter cars using fuel type and seating capacity.

### Car Comparison
Tested whether the chatbot could compare two vehicle models using the specifications available in the dataset.

### Missing Data Handling
Tested how the chatbot responded when a requested car was absent from the dataset or a vehicle's price was unavailable.

### EMI Calculation
Tested the EMI calculator against the applicable loan amount, interest rate, and repayment tenure.

## 5. Test Summary

- Total test cases: 6
- Passed: 6
- Failed: 0
- Initial test pass rate: 100%

**Pass rate = (Passed test cases ÷ Total test cases) × 100**

The six tested scenarios passed during the initial testing performed on the chatbot. These results reflect the scenarios tested and do not guarantee that every possible input will produce correct results.

## 6. Limitations

- Vehicle information depends on the uploaded datasets and configured knowledge sources.
- Dataset accuracy and completeness affect the quality of recommendations.
- Vehicle prices, specifications, and availability may change.
- EMI estimates may exclude additional charges unless explicitly included.
- Broader testing is required to evaluate unusual inputs and edge cases.

## 7. Future Testing Improvements

- Test additional budget ranges and fuel types.
- Test comparisons involving incomplete vehicle records.
- Validate EMI calculations using multiple loan scenarios.
- Test ambiguous user questions and spelling variations.
- Recheck results when the car datasets are updated.

---

**Project:** Dream Car Finder  
**Developer:** Pratik Thange  
**Platform:** Botpress
