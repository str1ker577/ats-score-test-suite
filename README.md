# ATS Scoring QA Test Suite

## Overview
This repository contains a QA test suite for the **ATS Scoring feature** of the CeeVee platform.

The objective is to evaluate:
- Scoring accuracy
- Keyword detection
- Suggestion quality
- Overall system reliability

---

##  Test Scope
Only the **ATS Scoring feature** is tested.

Inputs:
- Resume (PDF)
- Job Description (AI Engineer role)

Outputs evaluated:
- ATS Match Score
- Missing Keywords
- Recommendations

---

## Test Strategy

Three resumes were created to simulate different levels of relevance:

| Resume Type | Description |
|------------|------------|
| Complete | Highly aligned with job description |
| Partial | Moderately aligned |
| Minimal | Low relevance baseline |

---

## Repository Structure

---

## Test Documentation

See full report:  
**ATS_Test_Cases.md**

---

## Key Findings

### Strengths
- Accurate score scaling across resume quality levels  
- Clear differentiation between strong, moderate, and weak resumes  

### Issues Identified
- Exact keyword matching bias  
- Weak semantic understanding  
- False positives and false negatives  
- Occasional incorrect suggestions  

---

## Test Data Note
The resumes used in this project were **generated using AI tools** for the purpose of testing ATS behavior.

They are not real individuals.

---

## How to Reproduce

1. Open CeeVee ATS Scoring feature  
2. Upload a resume from `/resumes`  
3. Paste the job description  
4. Click Analyze  
5. Compare results with documented outputs  

---

## Conclusion

This project demonstrates practical QA testing of an AI-powered system, focusing not only on functionality but also on **system intelligence, reliability, and trustworthiness**.


Author: Kyle Hendrik Lee Lim
