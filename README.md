# Surveyor-Supreme - Enhancing Survey Insight and Effectiveness 

## Project Summary
The objective is to develop an internal analytics tool that helps surveyors and research teams extract meaningful insights from survey responses and improve survey quality. Potential approaches include data visualisation, machine learning, unsupervised learning, and large language models (LLMs), though other methods may also be applied.
The tool will support surveyors in understanding respondent behaviour, identifying weaknesses in survey design, and synthesising insights from both structured and unstructured responses. Ultimately, the solution aims to transform raw survey data into actionable, interpretable intelligence that can be used in day-to-day survey operations.




## Problem Statement
Creating a prototype that assists companies in analysing survey responses, improving survey design, and generating actionable insights for internal uses.
The solution should allow users to:
●	Identify patterns, correlations, or redundancies in survey questions that suggest opportunities for improvement

●	Understand factors associated with partial or incomplete survey responses

●	Discover meaningful demographic or behavioural segments among respondents

●	Extract insights from the applicant’s perspective on what drives employer attractiveness

●	Automatically synthesise and present insights in a clear and interpretable format, potentially using LLMs

## Workflow
![Workflow](./FlowChart.png)

## Dataset Overview

The dataset comprises anonymised GRADSG survey responses examining students' and graduates' perceptions of employers, career motivations, and information needs. Each record contains demographic variables (institution, field of study, nationality, gender), key outcome measures including employer attractiveness ratings (1-10 scale), and multi-select questions capturing priorities across career progression, compensation, work-life balance, and organizational culture. Operational metadata including timestamps, completion status, and geographic indicators enable analysis of survey completion behaviour and response patterns.

## Key Insights
This analysis reveals that employer attractiveness is primarily driven by respondents' educational identity (institution and field of study) and their current perception of the organization, rather than demographics or isolated motivational factors. 
The survey contains significant redundancy, with near-duplicate constructs appearing across multiple questions (e.g., "work-life balance" vs. "work-life balance and culture"), violating efficient survey design principles. 
Geographical clustering identifies three distinct recruitment segments, which are high-engagement clusters ready for conversion, awareness-gap clusters requiring brand-building, and misaligned clusters needing strategic reassessment. Each segment has different motivational priorities that demand tailored rather than uniform recruitment approaches.


## Setup

### 1. Create a Virtual Environment
```bash
# Create a virtual environment named 'venv'
python -m venv venv
```

### 2. Activate the Environment

**Mac / Linux:**
```bash
source venv/bin/activate
```

**Windows:**
```
# In Command Prompt
venv\Scripts\activate
# In PowerShell
venv\Scripts\Activate.ps1
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```


## How to Run

1. **Initialize Kernel**: Open `main.ipynb` and select the virtual environment (`venv`) as your Jupyter kernel.
2. **Execute**: Press **Run All** to execute all cells and generate the analysis and results.

## Project Folder Structure
```text
├── README.md              # Project summary and setup instructions
├── requirements.txt       # Project dependencies
├── .gitignore             # Files to exclude from Git
│
├── data/
│   ├── sds_datathon_gradsingapore.xlsx             # Immutable original data
│
├── main.ipynb
```
