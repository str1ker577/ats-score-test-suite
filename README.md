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

1. Review the job description and optimization inputs:
   - Open `/resumes/JD_and_Optimization_Input.pdf`

2. Open the CeeVee ATS Scoring feature

3. Upload one of the resumes:
   - `/resumes/AI_Engineer_Complete.pdf`
   - `/resumes/AI_Engineer_Partial.pdf`
   - `/resumes/AI_Engineer_Minimal.pdf`

4. Paste the same job description used in the reference file

5. Click **Analyze**

6. Compare results with:
   - `/ATS_Test_Cases.md`
   - `/screenshots/`

---

## Conclusion

This project demonstrates practical QA testing of an AI-powered system, focusing not only on functionality but also on **system intelligence, reliability, and trustworthiness**.


Author: Kyle Hendrik Lee Lim
