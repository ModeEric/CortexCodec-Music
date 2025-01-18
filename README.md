# EEG Music Analysis Research Project

Welcome to the EEG Music Analysis Research Project! This repository outlines the structured plan for our research aimed at analyzing EEG recordings in conjunction with music listening data. The ultimate goal is to produce a high-quality publication for a conference such as ISMIR.

## Table of Contents

- [Project Overview](#project-overview)
- [Teams](#teams)
- [Week-by-Week Task Breakdown](#week-by-week-task-breakdown)
  - [Week 1: Project Kickoff & Background Research](#week-1-project-kickoff--background-research)
  - [Week 2: Dataset Familiarization & Exploration](#week-2-dataset-familiarization--exploration)
  - [Week 3: Basic EEG Preprocessing](#week-3-basic-eeg-preprocessing)
  - [Week 4: Exploratory Data Analysis (EDA)](#week-4-exploratory-data-analysis-eda)
  - [Week 5: Feature Engineering](#week-5-feature-engineering)
  - [Week 6: Deeper Exploratory Analysis & Visualization](#week-6-deeper-exploratory-analysis--visualization)
  - [Week 7: Model Building (Classification or Regression)](#week-7-model-building-classification-or-regression)
  - [Week 8: Advanced Modeling & Refinement](#week-8-advanced-modeling--refinement)
  - [Week 9: Statistical Validation & Replicability Checks](#week-9-statistical-validation--replicability-checks)
  - [Week 10: Results Consolidation & Paper Outline](#week-10-results-consolidation--paper-outline)
  - [Week 11: Draft Writing & Revisions](#week-11-draft-writing--revisions)
  - [Week 12: Finalizing & Submission Preparation](#week-12-finalizing--submission-preparation)
- [General Best Practices](#general-best-practices)
- [Final Notes](#final-notes)

---

## Project Overview

This project involves analyzing EEG recordings taken while participants listen to various songs. The objective is to uncover relationships between brainwave activity and musical features, ultimately contributing to the field of Music Information Retrieval (MIR) and neuroscience. The project is structured into weekly sprints, each with clearly defined tasks assigned to specialized teams.

## Teams

To ensure efficient task management and expertise utilization, the project is divided into three specialized teams:

1. **Feature Extraction Team**
   - Focuses on extracting relevant features from both EEG and music data.
   
2. **Neuroscience Team**
   - Handles tasks related to EEG signal properties, preprocessing, and exploratory analysis from a neuroscience perspective.
   
3. **AI/ML Team**
   - Responsible for modeling, statistical analysis, and machine learning tasks to analyze the relationship between EEG and musical features.

Each team collaborates closely to ensure seamless integration of their work towards the common project goals.

## Week-by-Week Task Breakdown

### Week 1: Project Kickoff & Background Research

**Goals:**
- Understand project scope, objectives, and timeline.
- Assign roles and establish communication channels.

**Tasks:**

1. **Organize Kickoff Meeting**
   - **Team:** All Teams
   - **Description:** Schedule and conduct the kickoff meeting to discuss project goals, milestones, tools, and data access procedures.
   
2. **Set Up Version Control & Communication Channels**
   - **Team:** Feature Extraction Team
   - **Description:** Create a GitHub repository for code, notebooks, and documentation. Set up a shared folder (e.g., Google Drive) and communication channels (e.g., Slack).

3. **Assign Background Reading**
   - **Team:** Neuroscience Team & Feature Extraction Team
   - **Description:**
     - **Neuroscience Team:** Read introductory EEG references (e.g., chapters 1–2 of *“EEG Signal Processing”*) and summarize key points.
     - **Feature Extraction Team:** Read overviews of Music Information Retrieval tasks (e.g., chapters from *“Music Information Retrieval: Concepts, Techniques, and Applications”*) and summarize relevant content.
     - **AI/ML Team:** Find and summarize 2–3 papers on EEG + music research from IEEE or relevant journals.

4. **Conduct Group Discussion**
   - **Team:** All Teams
   - **Description:** Share summaries from background readings and upload them to the shared repository.

---

### Week 2: Dataset Familiarization & Exploration

**Goals:**
- Understand dataset structure and perform basic exploration.

**Tasks:**

1. **Data Inventory**
   - **Team:** Feature Extraction Team
   - **Description:** Catalog data files (format, number of subjects, total recordings, length, naming conventions) and document in a “Dataset Overview” markdown file.

2. **Preliminary Exploration**
   - **Team:** Neuroscience Team
   - **Description:** Write a Python/Jupyter notebook to load EEG data, plot raw signals for a few sessions, and check for sampling rates and artifacts. Add the notebook to GitHub with explanations.

3. **Audio Metadata Collection**
   - **Team:** Feature Extraction Team
   - **Description:** Gather metadata for each audio track (title, artist, genre, tempo, key, etc.), create a CSV or JSON summary, and document linkage to EEG recordings.

4. **Team Check-in**
   - **Team:** All Teams
   - **Description:** Ensure all members can load and plot data, and address any issues encountered.

---

### Week 3: Basic EEG Preprocessing

**Goals:**
- Introduce EEG preprocessing techniques.

**Tasks:**

1. **Literature Review on Preprocessing**
   - **Team:** Neuroscience Team
   - **Description:** Present a summary on common EEG preprocessing steps (e.g., band-pass filtering, notch filtering, ICA for artifact removal).

2. **Filter Implementation**
   - **Team:** Feature Extraction Team
   - **Description:** Implement a band-pass filter (e.g., 1–50 Hz) on a subset of data in a Jupyter notebook. Demonstrate before-and-after effects with plots.

3. **Artifact Removal**
   - **Team:** Neuroscience Team
   - **Description:** Investigate automated artifact removal approaches (e.g., ICA or threshold-based) and write a notebook function to detect and remove artifacts.

4. **Documentation**
   - **Team:** Feature Extraction Team
   - **Description:** Update README with preprocessing instructions and commit well-documented code to GitHub.

---

### Week 4: Exploratory Data Analysis (EDA)

**Goals:**
- Gain insights from EEG signals and identify data issues.

**Tasks:**

1. **Basic Statistical Analysis**
   - **Team:** Neuroscience Team
   - **Description:** Calculate mean, variance, and range of EEG signals per channel and subject. Summarize in a table and highlight anomalies.

2. **Time-Frequency Analysis**
   - **Team:** Neuroscience Team
   - **Description:** Compute and visualize power spectral density (PSD) in standard EEG bands (delta, theta, alpha, beta, gamma) for several recordings. Compare across different songs.

3. **Music Feature Exploration**
   - **Team:** Feature Extraction Team
   - **Description:** Extract musical features (tempo, key, energy, spectral features) using libraries like `librosa` and create summary statistics.

4. **Correlational Analysis**
   - **Team:** AI/ML Team
   - **Description:** Brainstorm potential correlations (e.g., alpha band power vs. track tempo) and document preliminary trends.

---

### Week 5: Feature Engineering

**Goals:**
- Identify and compute relevant EEG and music features.

**Tasks:**

1. **EEG Feature Extraction**
   - **Team:** Feature Extraction Team
   - **Description:** Implement functions to compute average band power (delta, theta, alpha, beta, gamma) for each recording segment. Explore additional features like phase locking value (PLV) or coherence.

2. **Segmenting EEG Data by Song Sections**
   - **Team:** Neuroscience Team
   - **Description:** Segment EEG data by song sections (e.g., verse, chorus) or time windows aligned with musical changes. Document segment labeling.

3. **Audio Feature Refinements**
   - **Team:** Feature Extraction Team
   - **Description:** Extract advanced musical features (spectral centroid, bandwidth, roll-off, zero-crossing rate, MFCCs) and organize them into a structured format (CSV/Pandas DataFrame).

4. **Version Control & Documentation**
   - **Team:** All Teams
   - **Description:** Update repository with new feature extraction scripts, ensure minimal code duplication, and write comprehensive docstrings.

---

### Week 6: Deeper Exploratory Analysis & Visualization

**Goals:**
- Investigate relationships between EEG and audio features and create visualizations.

**Tasks:**

1. **Correlation / Statistical Analysis**
   - **Team:** AI/ML Team
   - **Description:** Perform correlation analysis (Pearson, Spearman) between EEG band power and music features. Visualize using heatmaps or correlation plots.

2. **Dimensionality Reduction**
   - **Team:** AI/ML Team
   - **Description:** Apply PCA or t-SNE on combined EEG and music feature space to identify patterns or clusters. Document clustering observations.

3. **Data Visualization**
   - **Team:** Feature Extraction Team & Neuroscience Team
   - **Description:** Create various plots (boxplots, bar charts, time-series overlays) to illustrate key findings. Ensure clarity with well-labeled axes and annotations.

4. **Summary & Next Steps**
   - **Team:** All Teams
   - **Description:** Hold a group meeting to interpret findings and decide on relationships worth modeling further.

---

### Week 7: Model Building (Classification or Regression)

**Goals:**
- Design and implement initial modeling approaches based on findings.

**Tasks:**

1. **Model Definition**
   - **Team:** AI/ML Team
   - **Description:** Define a classification or regression task (e.g., predicting song preference from EEG alpha power). Clearly define input features and target variables.

2. **Train-Test Split**
   - **Team:** AI/ML Team
   - **Description:** Split data into training, validation, and test sets ensuring no data leakage (e.g., same participant or song across splits). Document the methodology.

3. **Baseline Models**
   - **Team:** AI/ML Team
   - **Description:** Implement simple baseline models (e.g., logistic regression, SVM) and evaluate using standard metrics (accuracy, F1-score, RMSE).

4. **Hyperparameter Tuning**
   - **Team:** AI/ML Team
   - **Description:** Set up grid search or cross-validation for hyperparameter tuning. Record best parameters and performance results.

---

### Week 8: Advanced Modeling & Refinement

**Goals:**
- Explore advanced models and refine feature selection and hyperparameters.

**Tasks:**

1. **Advanced Model Exploration**
   - **Team:** AI/ML Team
   - **Description:** Implement ensemble methods (Random Forest, XGBoost) or neural networks. Compare performance with baseline models.

2. **Feature Importance**
   - **Team:** AI/ML Team
   - **Description:** Investigate feature importance using techniques like permutation importance or random forest feature importance. Document findings with tables/plots.

3. **Model Refinement**
   - **Team:** AI/ML Team
   - **Description:** Apply feature selection or dimensionality reduction (e.g., Lasso, PCA) to mitigate overfitting. Summarize improvements or challenges.

4. **Intermediate Milestone Meeting**
   - **Team:** All Teams
   - **Description:** Decide on the final modeling approach for the paper and outline any additional necessary analyses.

---

### Week 9: Statistical Validation & Replicability Checks

**Goals:**
- Strengthen findings with statistical tests and ensure reproducibility.

**Tasks:**

1. **Statistical Tests**
   - **Team:** Neuroscience Team & AI/ML Team
   - **Description:** Conduct t-tests or ANOVAs where appropriate (e.g., EEG band differences across music genres). Document p-values and effect sizes in the required format.

2. **Cross-Validation & Reliability**
   - **Team:** AI/ML Team
   - **Description:** Perform k-fold cross-validation on the final model to confirm reliability. Summarize results in a report.

3. **Replicability**
   - **Team:** Feature Extraction Team
   - **Description:** Ensure all scripts can run in a fresh environment with minimal setup. Update `requirements.txt` or `environment.yml` for reproducibility.

4. **Internal Code Review**
   - **Team:** All Teams
   - **Description:** Review each other's code for clarity, modularity, and documentation. Address any issues collaboratively via GitHub.

---

### Week 10: Results Consolidation & Paper Outline

**Goals:**
- Consolidate results and create a draft outline for the publication.

**Tasks:**

1. **Organize Figures & Tables**
   - **Team:** Feature Extraction Team & Neuroscience Team
   - **Description:** Create a “results” folder with clearly named plots and tables. Ensure each figure includes a descriptive caption.

2. **Paper Outline**
   - **Team:** AI/ML Team
   - **Description:** Draft a detailed outline covering Introduction, Dataset & Methods, Results & Discussion, and Conclusions & Future Work. Share for group feedback.

3. **Methodology Write-Up**
   - **Team:** Neuroscience Team & AI/ML Team
   - **Description:** Begin drafting sections on data collection, preprocessing, feature engineering, and modeling approaches. Cite all relevant references.

4. **Meeting with Professor**
   - **Team:** All Teams
   - **Description:** Review the overall structure, confirm next steps for finalizing the paper, and identify any gaps to address in the final weeks.

---

### Week 11: Draft Writing & Revisions

**Goals:**
- Complete a near-final draft of the paper and incorporate feedback.

**Tasks:**

1. **Full Draft**
   - **Team:** All Teams
   - **Description:** Each team member takes a section (Introduction, Methods, Results, Conclusion) and contributes to the combined document (e.g., Google Docs or Overleaf).

2. **Editing & Consistency**
   - **Team:** All Teams
   - **Description:** Ensure consistent citation style, figure labeling, and clarity across all sections. Proofread for grammar and coherence.

3. **Collect Feedback**
   - **Team:** All Teams
   - **Description:** Share the draft with the professor and possibly external colleagues. Gather and incorporate feedback using tracked changes or comments.

4. **Plan Revisions**
   - **Team:** All Teams
   - **Description:** Prioritize and address feedback critical for publication acceptance, focusing on methodological clarity, thorough results, and relevant discussion.

---

### Week 12: Finalizing & Submission Preparation

**Goals:**
- Finalize the manuscript and prepare for submission.

**Tasks:**

1. **Implement Final Feedback**
   - **Team:** All Teams
   - **Description:** Resolve outstanding comments, finalize references, and ensure formatting adheres to the official conference template.

2. **Create Presentation**
   - **Team:** Feature Extraction Team & AI/ML Team
   - **Description:** Design a 10–12 slide deck summarizing key findings for conference presentation. Ensure all team members can present any slide.

3. **Double-Check Submission Requirements**
   - **Team:** AI/ML Team
   - **Description:** Verify word/page limits, style guidelines, and submission portal details. Validate PDF compliance (fonts embedded, figure resolution).

4. **Submission & Archiving**
   - **Team:** All Teams
   - **Description:** Submit the final paper to the conference. Archive all code, data references, and final documents in GitHub and/or a secure drive.

---

## General Best Practices

- **Version Control:** Commit early and often. Use pull requests for major changes and conduct code reviews.
- **Documentation:** Each script/notebook should include a description, purpose, and usage instructions.
- **Coding Standards:** Follow PEP 8 style guidelines for Python code or the equivalent for other languages.
- **Regular Meetings:** Hold weekly check-ins to track progress, identify blockers, and reassign tasks as necessary.
- **Backup Data:** Maintain offsite or cloud backups of critical raw and processed data.
- **Ethical & Responsible Research:** Ensure compliance with IRB or data privacy requirements for EEG research.

---

## Final Notes

- **Flexibility:** This schedule serves as a template and can be adjusted based on student availability, dataset complexity, and conference deadlines.
- **Communication:** Maintain consistent communication through weekly check-ins, clear GitHub issues, and a running task list to ensure all team members stay on track.
- **Encourage Initiative:** Allow students to take on additional exploratory tasks if they show aptitude or interest in advanced methods (e.g., deep learning, advanced signal processing).

With this structured plan, our teams will collaboratively progress from foundational understanding to data exploration, feature extraction, modeling, and finally, manuscript preparation and submission. Let’s work together to achieve a successful publication!

---

**Good luck to everyone involved!**

