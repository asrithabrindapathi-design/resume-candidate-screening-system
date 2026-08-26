# Resume & Candidate Screening System Using Machine Learning

## 📌 Project Overview

This project was developed as part of **Future Interns – Machine Learning Task 3 (2026)**.

The goal of this project is to build an intelligent resume screening system that automatically compares candidate resumes with a target job description, evaluates their suitability, ranks candidates based on job fit, and identifies missing skills.

The system demonstrates how NLP and Machine Learning techniques can support recruiters by reducing manual resume screening and providing an explainable candidate ranking.

## 🎯 Objectives

* Process and clean unstructured resume text
* Define job requirements and required skills
* Extract relevant skills from resumes
* Calculate resume-to-job similarity
* Generate candidate match scores
* Rank candidates according to role fit
* Identify missing skills
* Visualize candidate rankings

## 📊 Dataset

The project uses the **Resume Dataset**, containing **2,484 resumes** across multiple job categories.

Important columns include:

* `ID` – Unique resume identifier
* `Resume_str` – Resume text
* `Resume_html` – HTML representation of the resume
* `Category` – Resume/job category

The `Resume_str` column was used for text processing and candidate screening.

## 🛠️ Technologies Used

* Python
* Google Colab
* Pandas
* Matplotlib
* Scikit-learn
* TF-IDF
* Cosine Similarity
* Natural Language Processing (NLP)

## 🔄 Project Workflow

### 1. Data Loading

The resume dataset was loaded into a Pandas DataFrame.

### 2. Text Preprocessing

Resume text was cleaned by:

* Converting text to lowercase
* Removing punctuation and special characters
* Removing unnecessary whitespace
* Handling missing resume text
* Removing duplicate resumes

### 3. Job Description

A target **Software Engineer** job description was defined with required skills including:

* Python
* Java
* SQL
* Machine Learning
* Data Structures
* Algorithms
* Git
* Problem Solving
* Cloud Computing
* APIs
* Software Development

### 4. TF-IDF Feature Extraction

TF-IDF was used to convert the job description and resume text into numerical representations.

### 5. Resume-to-Job Similarity

**Cosine Similarity** was used to measure how closely each resume matches the target job description.

### 6. Skill Matching

The system checks each resume for the required skills and calculates a skill match percentage.

### 7. Candidate Scoring

The final candidate score is calculated using:

**Final Score = 60% Similarity Score + 40% Skill Match Score**

This provides a simple and explainable ranking mechanism.

### 8. Candidate Ranking

Candidates are sorted based on their final match score, allowing recruiters to quickly identify the strongest matches.

### 9. Skill Gap Identification

The system identifies required skills that are not found in each candidate's resume.

### 10. Visualization

A bar chart is generated to compare the top candidates based on their final match scores.

## 📈 Output

The system provides:

* Candidate rank
* Resume category
* Similarity score
* Skill match score
* Final match score
* Matched skills
* Missing skills

It also displays the best-ranked candidate and provides an overall explanation of their job fit.

## 💼 Business Applications

A system like this can help recruitment teams:

* Screen large numbers of resumes faster
* Shortlist candidates
* Identify candidates with relevant skills
* Highlight skill gaps
* Reduce manual screening effort
* Support consistent candidate evaluation

## 🚀 Future Improvements

The system can be enhanced by:

* Adding PDF resume parsing
* Supporting multiple job descriptions
* Using advanced NLP models such as BERT
* Adding experience-based scoring
* Weighting critical skills differently
* Building an interactive recruiter dashboard
* Adding explainable candidate recommendations
* Integrating the system with an applicant tracking system (ATS)

## 📌 Key Learning

This project provided hands-on experience with **NLP, TF-IDF, cosine similarity, skill matching, candidate ranking, and explainable Machine Learning applications in recruitment**.

## 👩‍💻 Internship

**Future Interns – Machine Learning Task 3**

**Task:** Resume / Candidate Screening System

**Platform:** Google Colab

---

⭐ This project demonstrates how NLP and Machine Learning can be applied to automate and support real-world recruitment workflows.
