# EEG Music Analysis Research Project

Welcome to the EEG Music Analysis Research Project! This repository outlines our structured plan for the ongoing research aimed at analyzing EEG recordings in conjunction with music listening data. Building on the work from the previous semester, our goal this semester is to **investigate the relationship between musical features and EEG band power to predict listener engagement**. The culmination of this project will be a high-quality publication for a conference such as ISMIR.

## Table of Contents

- [Project Overview](#project-overview)
- [Research Objective](#research-objective)
- [Hypotheses](#hypotheses)
- [Methodology](#methodology)
- [Teams](#teams)
- [Week-by-Week Task Breakdown](#week-by-week-task-breakdown)
  - [Week 1: Project Kickoff & Background Review](#week-1-project-kickoff--background-review)
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

This project involves analyzing EEG recordings taken while participants listen to various songs. Building upon the literature reviews and preliminary work completed last semester, this semester's focus is on **investigating how specific musical features influence EEG band power** and leveraging this relationship to **predict listener engagement**. Our interdisciplinary approach combines expertise in feature extraction, neuroscience, and machine learning to achieve these objectives.

## Research Objective

To explore and quantify the relationship between musical features (such as tempo, key, harmony) and EEG band power (delta, theta, alpha, beta, gamma) to develop predictive models of listener engagement during music listening sessions.

## Hypotheses

1. **H1:** Higher tempo in music is positively correlated with increased beta and gamma band power in EEG signals.
2. **H2:** Specific musical keys are associated with distinct patterns in alpha band power, reflecting varying levels of listener relaxation or alertness.
3. **H3:** A combination of musical and EEG features can effectively predict listener engagement levels with an accuracy exceeding baseline models.

## Methodology

1. **Data Collection:** Utilize the existing dataset of EEG recordings synchronized with music listening sessions.
2. **Preprocessing:** Apply standard EEG preprocessing techniques, including band-pass filtering and artifact removal.
3. **Feature Extraction:** Extract relevant musical features using `librosa` and EEG features such as band power using `MNE`.
4. **Exploratory Analysis:** Perform statistical analyses to identify correlations and patterns between musical and EEG features.
5. **Modeling:** Develop machine learning models to predict listener engagement based on the extracted features.
6. **Validation:** Validate models using cross-validation and statistical tests to ensure reliability and replicability.
7. **Publication:** Consolidate findings into a manuscript suitable for submission to ISMIR.

## Teams

To ensure efficient task management and leverage specialized expertise, the project is divided into three focused teams:

1. **Feature Extraction Team**
   - **Responsibilities:** Extracting relevant features from both EEG and music data, handling data inventory, and managing audio metadata.
   
2. **Neuroscience Team**
   - **Responsibilities:** Handling EEG signal properties, preprocessing, exploratory analysis from a neuroscience perspective, and artifact identification.
   
3. **AI/ML Team**
   - **Responsibilities:** Developing and refining machine learning models, performing statistical analyses, and integrating EEG and audio features for predictive tasks.

Each team collaborates closely, ensuring seamless integration of their work towards the common project objectives.

---

## Week-by-Week Task Breakdown

### Week 1: Project Kickoff & Background Review

**Goals:**
- Align all teams on the current project status and objectives for the semester.
- Review existing literature summaries from each team and identify areas requiring deeper understanding or further exploration.
- Establish clear roles and responsibilities.

**Tasks:**

#### **All Teams**

1. **Organize Kickoff Meeting**
   - **Description:** Conduct a meeting to:
     - Provide an overview of the project progress to date.
     - Recap key findings from last semester’s work.
     - Outline this semester’s goals and timeline.
     - Assign roles and responsibilities to each team.

2. **Review Existing Literature Summaries**
   - **Description:** Each team reviews the literature summaries they prepared last semester and identifies:
     - Key methodologies or findings directly relevant to their tasks.
     - Gaps or unclear areas that require further exploration.
     - Actionable insights for feature extraction, neuroscience analysis, or AI/ML modeling.

#### **Homework for Next Meeting**

- **Neuroscience Team:**
  - Review existing preprocessing methods and artifact removal strategies.
  - Identify any gaps or potential improvements.

- **Feature Extraction Team:**
  - Research recent developments in audio feature extraction for music analysis.
  - Note specific methods that could apply to this dataset.

- **AI/ML Team:**
  - Investigate advanced modeling techniques for integrating EEG and audio features, such as multimodal learning frameworks.

**Deliverables:**
- Meeting notes summarizing roles, objectives, and milestones.
- A short document or slide deck summarizing the most relevant insights and any new papers to investigate.
- A shared document listing assigned follow-up readings and their rationale.

---

### Week 2: Dataset Familiarization & Exploration

**Goals:**
- Understand the dataset structure and perform basic exploration to prepare for deeper analysis.

**Tasks:**

#### **Feature Extraction Team**

1. **Data Inventory**
   - **Description:** Catalog the data files by documenting:
     - File formats
     - Number of subjects
     - Total recordings
     - Length of recordings
     - Naming conventions
   - **Deliverable:** A “Dataset Overview” markdown file added to the GitHub repository.

2. **Audio Metadata Collection**
   - **Description:** Gather metadata for each audio track, including:
     - Title
     - Artist
     - Genre
     - Tempo
     - Key
   - Create a summary in a structured format (e.g., CSV or JSON) and ensure proper linkage to EEG recordings.
   - **Deliverable:** A metadata summary file added to the repository.

#### **Neuroscience Team**

1. **Preliminary Exploration**
   - **Description:** Create a Python/Jupyter notebook to:
     - Load EEG data.
     - Plot raw signals for a few sessions to observe patterns and check for sampling rates or artifacts.
   - **Deliverable:** A Jupyter notebook added to the GitHub repository with clear explanations and sample visualizations.

2. **Artifact Identification**
   - **Description:** Begin researching common EEG artifacts (e.g., eye blinks, muscle movements) and note how they might appear in the dataset.
   - **Deliverable:** A short document or markdown file summarizing key artifact characteristics and potential preprocessing methods to address them.

#### **AI/ML Team**

1. **Dataset Familiarization**
   - **Description:** Explore how EEG data and audio metadata will eventually connect for machine learning tasks. Tasks include:
     - Reviewing the “Dataset Overview” markdown from the Feature Extraction Team.
     - Analyzing metadata fields to understand their potential use as features for modeling.
   - **Deliverable:** A markdown file or comments summarizing initial observations and suggestions for preprocessing or feature extraction.

2. **Begin Learning Frameworks**
   - **Description:** Start exploring tools and frameworks for EEG-related machine learning tasks, such as:
     - Libraries like MNE, PyTorch, or scikit-learn.
     - Understanding common EEG machine learning preprocessing pipelines.
   - **Deliverable:** A brief document listing key libraries/tools, their potential use cases, and any installation/setup issues encountered.

#### **All Teams**

1. **Team Check-in**
   - **Description:** During the weekly meeting:
     - Ensure all members can load and plot data successfully.
     - Discuss and address any challenges or issues encountered during the week.
     - Share deliverables completed so far and ensure they are pushed to the GitHub repository.
   - **Deliverable:** Meeting notes summarizing progress and action items for Week 3.

---

### Week 3: Basic EEG Preprocessing

**Goals:**
- Introduce and implement foundational EEG preprocessing techniques to prepare the data for analysis.

**Tasks:**

#### **Feature Extraction Team**

1. **Implement Band-Pass Filtering**
   - **Description:** Write a Python/Jupyter notebook to:
     - Implement a band-pass filter (e.g., 1–50 Hz) for EEG signals.
     - Test the filter on a subset of the data.
     - Plot the before-and-after effects of the filter to demonstrate its impact.
   - **Deliverable:** A notebook added to the GitHub repository with well-documented code and sample visualizations.

2. **Document Filtering Process**
   - **Description:** Create a markdown file explaining:
     - The rationale for band-pass filtering.
     - The chosen filter parameters (e.g., cutoff frequencies).
     - Potential limitations of the approach.
   - **Deliverable:** A markdown file added to the repository.

#### **Neuroscience Team**

1. **Artifact Identification and Removal**
   - **Description:** Research and implement a basic artifact removal strategy:
     - Investigate methods such as Independent Component Analysis (ICA) or threshold-based approaches.
     - Write a Python/Jupyter notebook to detect and remove or label common artifacts in the dataset.
   - **Deliverable:** A notebook added to the GitHub repository with explanations and visualizations of artifact removal.

2. **Visualize Artifacts**
   - **Description:** Create visual examples of common EEG artifacts (e.g., eye blinks, muscle movements) using the dataset.
   - **Deliverable:** Annotated plots added to the repository for educational purposes.

#### **AI/ML Team**

1. **Understand EEG Preprocessing Techniques**
   - **Description:** Study the preprocessing techniques implemented by the Feature Extraction and Neuroscience Teams, including:
     - Band-pass filtering.
     - Artifact removal.
     - Time-frequency representations (if applicable).
   - **Deliverable:** A brief markdown summary explaining how these preprocessing steps will affect downstream machine learning tasks.

2. **Setup for EEG Feature Extraction**
   - **Description:** Start exploring tools and methods for extracting EEG features suitable for machine learning. Focus on:
     - Libraries like MNE or EEG-related extensions in PyTorch or TensorFlow.
     - Power spectral density (PSD) or band-specific power features.
   - **Deliverable:** Notes or a short report listing potential feature extraction methods.

#### **All Teams**

1. **Team Check-in**
   - **Description:** Conduct a check-in to:
     - Review progress on preprocessing tasks.
     - Address challenges or blockers in implementation.
     - Ensure that deliverables (notebooks, markdown files) are documented and uploaded to the repository.
   - **Deliverable:** Meeting notes summarizing the discussion and action items for Week 4.

---

### Week 4: Exploratory Data Analysis (EDA)

**Goals:**
- Gain insights into the EEG signals and audio metadata through statistical and visual analysis.
- Identify potential anomalies or areas needing further preprocessing.

**Tasks:**

#### **Feature Extraction Team**

1. **Audio Metadata Analysis**
   - **Description:** Perform an exploratory analysis of the audio metadata:
     - Calculate descriptive statistics (e.g., mean, median, standard deviation) for numerical features like tempo and key.
     - Visualize distributions of categorical metadata such as genres and keys.
     - Investigate missing or inconsistent metadata entries.
   - **Deliverable:** A Jupyter notebook with visualizations (e.g., histograms, bar plots) and a markdown summary of findings.

2. **Cross-Check Metadata with EEG Data**
   - **Description:** Ensure that all audio metadata is correctly linked to the EEG recordings.
     - Identify and document any missing or mismatched links between datasets.
   - **Deliverable:** Updated metadata file and a markdown report on linkage quality.

#### **Neuroscience Team**

1. **EEG Signal Analysis**
   - **Description:** Perform basic statistical analysis of EEG signals:
     - Calculate mean, variance, and standard deviation for each channel across sessions.
     - Identify potential anomalies such as extreme values or flatlined channels.
   - **Deliverable:** A Jupyter notebook summarizing the analysis with visualizations and tables.

2. **Time-Frequency Analysis**
   - **Description:** Compute power spectral density (PSD) for standard EEG frequency bands (delta, theta, alpha, beta, gamma) and visualize results for a few sessions.
     - Compare power spectral differences across sessions or channels.
   - **Deliverable:** A notebook with annotated plots and a markdown explanation of key findings.

#### **AI/ML Team**

1. **Correlational Analysis**
   - **Description:** Investigate correlations between EEG signals and audio metadata:
     - Focus on relationships like alpha band power vs. tempo or key.
     - Create visualizations (e.g., heatmaps) to highlight notable correlations.
   - **Deliverable:** A notebook with correlation matrices, plots, and an explanation of trends.

2. **Explore Dimensionality Reduction**
   - **Description:** Experiment with dimensionality reduction techniques (e.g., PCA, t-SNE) on EEG features or combined EEG and audio features.
     - Visualize clusters or patterns in the data to identify groupings or trends.
   - **Deliverable:** A notebook with dimensionality reduction analyses and visualizations.

#### **All Teams**

1. **Team Check-in**
   - **Description:** During the weekly meeting:
     - Share findings from exploratory analysis.
     - Discuss any challenges or anomalies observed in the datasets.
     - Plan adjustments to preprocessing or feature extraction based on EDA results.
   - **Deliverable:** Meeting notes summarizing key findings and action items for Week 5.

---

### Week 5: Feature Engineering

**Goals:**
- Identify and compute relevant EEG and music features.
- Continue refining the audio feature set.

**Tasks:**

#### **Feature Extraction Team**

1. **EEG Feature Extraction**
   - **Description:** Implement functions to compute average band power (delta, theta, alpha, beta, gamma) for each recording segment.
     - Explore additional features like phase locking value (PLV) or coherence if applicable.
   - **Deliverable:** A Jupyter notebook with feature extraction functions and sample outputs.

2. **Audio Feature Refinements**
   - **Description:** Extract advanced musical features (spectral centroid, bandwidth, roll-off, zero-crossing rate, MFCCs) using libraries like `librosa`.
     - Organize these features into a structured format (e.g., CSV or Pandas DataFrame).
   - **Deliverable:** A structured audio features file added to the repository.

#### **Neuroscience Team**

1. **Segmenting EEG Data by Song Sections**
   - **Description:** Segment EEG data by song sections (e.g., verse, chorus) or time windows aligned with musical changes.
     - Document how the segments are labeled in the dataset.
   - **Deliverable:** A markdown file detailing segmentation criteria and labeling methodology.

2. **Enhance EEG Feature Extraction**
   - **Description:** Collaborate with the AI/ML team to refine EEG features based on initial EDA findings.
     - Implement any additional EEG features identified as relevant during EDA.
   - **Deliverable:** Updated feature extraction scripts or notebooks.

#### **AI/ML Team**

1. **Feature Selection Planning**
   - **Description:** Based on EDA and feature extraction outputs, plan feature selection strategies for modeling.
     - Identify which EEG and audio features are most promising for predictive tasks.
   - **Deliverable:** A markdown document outlining proposed feature selection methods and criteria.

2. **Integrate EEG and Audio Features**
   - **Description:** Begin integrating EEG and audio features into a unified dataset suitable for machine learning tasks.
     - Ensure proper alignment and synchronization between EEG data segments and corresponding audio features.
   - **Deliverable:** An integrated dataset file ready for modeling, added to the repository.

#### **All Teams**

1. **Team Check-in**
   - **Description:** Conduct a check-in to:
     - Review progress on feature engineering tasks.
     - Address any integration challenges between EEG and audio features.
     - Ensure that all deliverables are documented and uploaded to the repository.
   - **Deliverable:** Meeting notes summarizing progress and action items for Week 6.

---

### Week 6: Deeper Exploratory Analysis & Visualization

**Goals:**
- Investigate relationships between EEG and audio features.
- Create intuitive data visualizations for group discussion.

**Tasks:**

#### **Feature Extraction Team**

1. **Advanced Audio Feature Analysis**
   - **Description:** Dive deeper into the extracted audio features to identify patterns or anomalies.
     - Compare advanced features across different genres or artists.
   - **Deliverable:** A Jupyter notebook with detailed analysis and visualizations of advanced audio features.

2. **Integrate Additional Features**
   - **Description:** Incorporate any new audio features identified as beneficial during the previous week's analysis.
     - Update the audio features dataset accordingly.
   - **Deliverable:** Updated audio features file with additional features added.

#### **Neuroscience Team**

1. **Advanced EEG Signal Analysis**
   - **Description:** Perform more in-depth statistical analyses on EEG signals, such as:
     - Time-frequency analysis across different segments.
     - Cross-channel correlations or connectivity measures.
   - **Deliverable:** A notebook with advanced EEG analyses and corresponding visualizations.

2. **Visualize EEG Features**
   - **Description:** Create detailed visualizations of EEG features, such as:
     - Topographical maps of brain activity.
     - Time-series overlays of different frequency bands.
   - **Deliverable:** Annotated plots and figures added to the repository.

#### **AI/ML Team**

1. **Correlation / Statistical Analysis**
   - **Description:** Perform correlation analysis (Pearson, Spearman) between EEG band power and music features.
     - Visualize results in heatmaps or correlation plots to identify significant relationships.
   - **Deliverable:** A notebook with correlation matrices, plots, and an explanation of trends.

2. **Dimensionality Reduction**
   - **Description:** Apply PCA or t-SNE on the combined EEG and music feature space to identify patterns or clusters.
     - Document if certain songs or EEG states cluster together.
   - **Deliverable:** A notebook with dimensionality reduction analyses and visualizations.

#### **All Teams**

1. **Team Check-in**
   - **Description:** During the weekly meeting:
     - Present and discuss findings from exploratory analyses.
     - Identify any surprising trends or patterns.
     - Decide on which relationships are worth modeling further.
   - **Deliverable:** Meeting notes summarizing key insights and planning for Week 7.

---

### Week 7: Model Building (Classification or Regression)

**Goals:**
- Design and implement initial modeling approaches based on exploratory findings.
- Develop a clear framework for machine learning tasks.

**Tasks:**

#### **Feature Extraction Team**

1. **Prepare Feature Sets for Modeling**
   - **Description:** Organize and clean the extracted EEG and audio features to ensure they are ready for machine learning tasks.
     - Handle any missing values or inconsistencies.
   - **Deliverable:** A cleaned and well-structured feature set added to the repository.

2. **Documentation of Feature Engineering**
   - **Description:** Document the feature engineering process, detailing:
     - Methods used for feature extraction.
     - Justifications for selected features.
     - Any challenges faced during feature preparation.
   - **Deliverable:** A comprehensive markdown file outlining the feature engineering steps.

#### **Neuroscience Team**

1. **Support Feature Integration**
   - **Description:** Collaborate with the Feature Extraction and AI/ML Teams to ensure EEG features are appropriately integrated with audio features.
     - Provide insights on the relevance of certain EEG features based on neuroscience principles.
   - **Deliverable:** A markdown file or comments in relevant notebooks providing collaborative insights.

2. **Prepare EEG Feature Documentation**
   - **Description:** Create detailed documentation of the EEG features being used for modeling, including:
     - Definitions and interpretations of each feature.
     - Potential implications for predictive tasks.
   - **Deliverable:** A markdown file added to the repository.

#### **AI/ML Team**

1. **Model Definition**
   - **Description:** Define a classification or regression task based on initial findings. For example:
     - **Classification:** Predicting listener engagement levels (e.g., high vs. low) based on EEG and musical features.
     - **Regression:** Predicting a continuous engagement score from EEG and musical features.
   - **Deliverable:** A markdown file clearly defining the modeling task, input features, and target variables.

2. **Train-Test Split**
   - **Description:** Split the integrated dataset into training, validation, and test sets.
     - Ensure no data leakage by keeping the same participant or song out of multiple splits.
     - Document the splitting methodology.
   - **Deliverable:** A Jupyter notebook detailing the train-test split process and rationale.

3. **Baseline Models**
   - **Description:** Implement simple baseline models (e.g., logistic regression for classification, linear regression for regression tasks).
     - Evaluate these models using standard metrics (accuracy, F1-score, RMSE, etc., depending on the task).
   - **Deliverable:** A notebook with baseline model implementations, evaluations, and results.

4. **Hyperparameter Tuning**
   - **Description:** Set up a basic grid search or cross-validation approach to tune model hyperparameters.
     - Record the best parameters and performance results.
   - **Deliverable:** A notebook or CSV file documenting hyperparameter tuning outcomes.

#### **All Teams**

1. **Team Check-in**
   - **Description:** During the weekly meeting:
     - Review progress on model building tasks.
     - Discuss baseline model performance and any initial observations.
     - Plan next steps for advanced modeling and feature refinement.
   - **Deliverable:** Meeting notes summarizing progress and action items for Week 8.

---

### Week 8: Advanced Modeling & Refinement

**Goals:**
- Explore advanced machine learning models.
- Refine feature selection and model hyperparameters for improved performance.

**Tasks:**

#### **Feature Extraction Team**

1. **Advanced Feature Engineering**
   - **Description:** Enhance EEG and audio features based on insights from modeling results.
     - Implement any additional feature extraction methods identified as beneficial.
   - **Deliverable:** Updated feature extraction scripts or notebooks with advanced features.

2. **Feature Normalization and Scaling**
   - **Description:** Apply normalization or scaling techniques to the feature sets to prepare for advanced modeling.
     - Document the methods used and their impact on feature distributions.
   - **Deliverable:** A notebook demonstrating feature scaling and its effects.

#### **Neuroscience Team**

1. **Provide Insights on Feature Importance**
   - **Description:** Collaborate with the AI/ML Team to interpret the importance of EEG features based on model outputs.
     - Offer neuroscience-based explanations for why certain features may be more predictive.
   - **Deliverable:** A markdown file or comments in relevant notebooks providing interpretative insights.

2. **Enhance Artifact Removal Techniques**
   - **Description:** Based on previous artifact identification, implement more robust artifact removal strategies if necessary.
     - Test these methods and assess their impact on data quality.
   - **Deliverable:** Updated preprocessing notebooks with enhanced artifact removal methods.

#### **AI/ML Team**

1. **Advanced Model Exploration**
   - **Description:** Implement and evaluate more complex models, such as:
     - Ensemble methods (Random Forest, XGBoost).
     - Neural networks (e.g., simple feedforward networks or CNNs for EEG data).
   - **Deliverable:** A notebook with advanced model implementations, evaluations, and comparative results against baseline models.

2. **Feature Importance Analysis**
   - **Description:** Investigate which features are most predictive using techniques like permutation importance or random forest feature importance.
     - Document these findings with clear tables or plots.
   - **Deliverable:** A notebook with feature importance analyses and corresponding visualizations.

3. **Model Refinement**
   - **Description:** Refine models by:
     - Applying feature selection or dimensionality reduction techniques (e.g., Lasso, PCA).
     - Addressing overfitting through regularization or other methods.
   - **Deliverable:** Updated modeling notebooks demonstrating refined models and improved performance metrics.

#### **All Teams**

1. **Intermediate Milestone Meeting**
   - **Description:** Conduct a meeting to:
     - Decide on the final modeling approach to be included in the paper.
     - Outline any additional analyses needed for clarity or completeness.
     - Assign tasks for any remaining refinements or explorations.
   - **Deliverable:** Meeting notes outlining the final modeling strategy and next steps for Week 9.

---

### Week 9: Statistical Validation & Replicability Checks

**Goals:**
- Strengthen the rigor of findings with proper statistical tests.
- Ensure reproducibility and clear code structure.

**Tasks:**

#### **Feature Extraction Team**

1. **Enhance Data Documentation**
   - **Description:** Ensure all feature extraction processes are thoroughly documented, including:
     - Steps taken.
     - Parameters used.
     - Rationale behind feature choices.
   - **Deliverable:** Comprehensive markdown documentation within the repository.

2. **Data Integrity Checks**
   - **Description:** Perform checks to ensure the integrity and consistency of the extracted features.
     - Identify and rectify any discrepancies or inconsistencies.
   - **Deliverable:** A report detailing data integrity findings and corrective actions taken.

#### **Neuroscience Team**

1. **Statistical Tests**
   - **Description:** Conduct statistical tests to validate EEG findings, such as:
     - T-tests or ANOVAs to compare EEG band powers across different music genres or conditions.
     - Calculate effect sizes and p-values.
   - **Deliverable:** A notebook with statistical test implementations, results, and interpretations.

2. **Cross-Validation & Reliability**
   - **Description:** Collaborate with the AI/ML Team to ensure that EEG preprocessing and feature extraction methods contribute to reliable model performance.
     - Validate that preprocessing steps do not introduce biases.
   - **Deliverable:** A markdown file summarizing reliability checks and their outcomes.

#### **AI/ML Team**

1. **Cross-Validation & Reliability**
   - **Description:** Perform k-fold cross-validation on the final model to confirm reliability and generalizability.
     - Summarize cross-validation results and assess model robustness.
   - **Deliverable:** A notebook with cross-validation implementations and summarized results.

2. **Replicability**
   - **Description:** Ensure that all scripts can be run in a fresh environment with minimal setup.
     - Update `requirements.txt` or `environment.yml` with all necessary dependencies.
   - **Deliverable:** Updated environment files added to the repository.

3. **Internal Code Review**
   - **Description:** Review the code of at least one other team member for clarity, modularity, and documentation.
     - File any issues in GitHub and address them collaboratively.
   - **Deliverable:** Code review comments and resolved issues documented within GitHub.

#### **All Teams**

1. **Team Check-in**
   - **Description:** During the weekly meeting:
     - Present statistical validation results.
     - Discuss replicability and code review outcomes.
     - Identify any remaining issues to address before results consolidation.
   - **Deliverable:** Meeting notes summarizing validation results and action items for Week 10.

---

### Week 10: Results Consolidation & Paper Outline

**Goals:**
- Consolidate all final figures, tables, and model results into a draft for publication.
- Create a formal outline matching ISMIR or similar conference template.

**Tasks:**

#### **Feature Extraction Team**

1. **Organize Figures & Tables**
   - **Description:** Compile all relevant figures and tables generated from feature extraction and analysis.
     - Ensure each figure is clearly named and includes descriptive captions.
   - **Deliverable:** A “results” folder within the repository containing all figures and tables.

2. **Prepare Feature Documentation for Paper**
   - **Description:** Summarize the feature extraction process, including:
     - Methods used.
     - Rationale for feature selection.
     - Any challenges or notable observations.
   - **Deliverable:** A markdown section or document ready to be included in the paper.

#### **Neuroscience Team**

1. **Document EEG Analysis Findings**
   - **Description:** Summarize key findings from EEG signal analysis and statistical tests.
     - Include interpretations from a neuroscience perspective.
   - **Deliverable:** A markdown section or document ready to be included in the paper.

2. **Prepare Visualization Assets**
   - **Description:** Ensure all visualizations related to EEG data are high-quality and publication-ready.
     - Optimize figures for clarity and compliance with conference guidelines.
   - **Deliverable:** Optimized figures added to the “results” folder.

#### **AI/ML Team**

1. **Paper Outline**
   - **Description:** Draft a detailed outline covering:
     - **Introduction:** Motivation, background, and prior work.
     - **Dataset & Methods:** Detailed description of datasets, preprocessing, feature extraction, and modeling approaches.
     - **Results & Discussion:** Presentation and interpretation of model results, statistical validations, and feature importance.
     - **Conclusions & Future Work:** Summarize findings and suggest areas for future research.
   - **Deliverable:** An outline document shared in the repository for group feedback.

2. **Methodology Write-Up**
   - **Description:** Begin drafting sections on:
     - Data collection (if conducted by a third party, mention that).
     - Preprocessing steps.
     - Feature engineering.
     - Modeling approach.
     - Cite all relevant references in standard format.
   - **Deliverable:** Initial draft sections added to the repository.

3. **Integrate Model Results**
   - **Description:** Compile model performance metrics and visualizations.
     - Prepare tables and plots to showcase model comparisons and best-performing models.
   - **Deliverable:** Model results added to the “results” folder and linked in the paper draft.

#### **All Teams**

1. **Meeting with Professor**
   - **Description:** Schedule a review meeting with the professor to:
     - Present the current paper outline and key findings.
     - Confirm the overall structure and direction.
     - Identify any gaps or additional analyses needed before drafting.
   - **Deliverable:** Meeting notes outlining feedback and required adjustments.

---

### Week 11: Draft Writing & Revisions

**Goals:**
- Complete a near-final draft of the paper.
- Incorporate feedback from the professor and peers.

**Tasks:**

#### **Feature Extraction Team**

1. **Contribute to Methods & Results Sections**
   - **Description:** Write detailed sections on:
     - Feature extraction processes.
     - Audio metadata analysis.
   - **Deliverable:** Sections added to the combined paper draft.

2. **Ensure Consistency in Figures**
   - **Description:** Verify that all figures related to feature extraction are consistently formatted and referenced in the text.
   - **Deliverable:** Updated figures and figure captions in the repository.

#### **Neuroscience Team**

1. **Contribute to Methods & Results Sections**
   - **Description:** Write detailed sections on:
     - EEG preprocessing techniques.
     - Statistical validation of EEG findings.
   - **Deliverable:** Sections added to the combined paper draft.

2. **Interpretation of Results**
   - **Description:** Provide neuroscientific interpretations of the EEG analysis results.
   - **Deliverable:** Written interpretations added to the Results & Discussion section.

#### **AI/ML Team**

1. **Contribute to Methods & Results Sections**
   - **Description:** Write detailed sections on:
     - Machine learning models used.
     - Model training and evaluation processes.
     - Feature importance and model comparisons.
   - **Deliverable:** Sections added to the combined paper draft.

2. **Integrate Statistical Results**
   - **Description:** Incorporate statistical validation results and their implications for the models.
   - **Deliverable:** Updated Results & Discussion section with statistical insights.

#### **All Teams**

1. **Full Draft Compilation**
   - **Description:** Combine all written sections into a single document (e.g., Google Docs or Overleaf).
     - Ensure seamless flow between sections and proper integration of figures and tables.
   - **Deliverable:** A complete draft of the paper ready for review.

2. **Editing & Consistency**
   - **Description:** 
     - Check for consistent citation style and formatting.
     - Ensure all figures and tables are properly labeled and referenced.
     - Proofread for grammar, clarity, and coherence.
   - **Deliverable:** A polished draft with consistent formatting and no grammatical errors.

3. **Collect Feedback**
   - **Description:** Share the draft with the professor and possibly external colleagues.
     - Gather feedback using tracked changes or comment threads.
   - **Deliverable:** Feedback collected and documented within the repository.

4. **Plan Revisions**
   - **Description:** Prioritize and address feedback critical for publication acceptance.
     - Focus on methodological clarity, thorough results, and relevant discussion.
   - **Deliverable:** A list of revisions and assigned tasks for implementing feedback.

---

### Week 12: Finalizing & Submission Preparation

**Goals:**
- Finalize the manuscript for submission to ISMIR (or a similar conference).
- Prepare presentation materials if required (e.g., slides or poster).

**Tasks:**

#### **Feature Extraction Team**

1. **Implement Final Feedback on Methods**
   - **Description:** Refine the feature extraction methods based on feedback.
     - Ensure all processes are clearly explained and justified in the manuscript.
   - **Deliverable:** Updated methods sections and feature extraction scripts.

2. **Prepare Final Figures**
   - **Description:** Ensure all feature-related figures are high-resolution and adhere to conference guidelines.
   - **Deliverable:** Finalized figures added to the “results” folder.

#### **Neuroscience Team**

1. **Implement Final Feedback on EEG Analysis**
   - **Description:** Refine EEG analysis sections based on feedback.
     - Clarify interpretations and ensure statistical results are accurately reported.
   - **Deliverable:** Updated EEG analysis sections in the manuscript.

2. **Finalize EEG Visualizations**
   - **Description:** Ensure all EEG-related figures are optimized for clarity and publication standards.
   - **Deliverable:** Finalized EEG visualizations added to the “results” folder.

#### **AI/ML Team**

1. **Implement Final Feedback on Modeling**
   - **Description:** Refine the modeling sections based on feedback.
     - Clarify model selection, feature importance, and statistical validations.
   - **Deliverable:** Updated modeling sections in the manuscript.

2. **Finalize Model Results Visualizations**
   - **Description:** Ensure all model-related figures and tables are polished and meet publication standards.
   - **Deliverable:** Finalized model results figures added to the “results” folder.

3. **Finalize Paper Outline**
   - **Description:** Ensure that the paper outline aligns with the final draft and conference requirements.
   - **Deliverable:** A finalized outline ready for final manuscript adjustments.

#### **All Teams**

1. **Implement Final Feedback**
   - **Description:** Resolve all outstanding comments and incorporate final feedback from the professor and peers.
     - Finalize references and ensure compliance with the conference template.
   - **Deliverable:** A polished manuscript ready for submission.

2. **Create Presentation**
   - **Description:** 
     - **Feature Extraction Team & AI/ML Team:** Design a 10–12 slide deck summarizing key findings.
     - Ensure that any team member can present any slide if needed.
   - **Deliverable:** Presentation slides added to the repository.

3. **Double-Check Submission Requirements**
   - **Description:** Verify that the manuscript adheres to all submission guidelines, including:
     - Word/page limits.
     - Formatting and style requirements.
     - Submission portal details.
   - **Deliverable:** A checklist ensuring all submission requirements are met.

4. **Submission & Archiving**
   - **Description:** 
     - Submit the final paper to the conference.
     - Archive all code, data references, and final documents in GitHub and/or a secure drive.
   - **Deliverable:** Confirmation of paper submission and archived materials.

---

## General Best Practices

- **Version Control:** Commit early and often. Use pull requests for major changes and conduct code reviews to maintain code quality.
- **Documentation:** Ensure each script/notebook includes a description, purpose, and usage instructions. Maintain comprehensive documentation for all processes.
- **Coding Standards:** Follow PEP 8 style guidelines for Python code or the equivalent for other programming languages to ensure readability and maintainability.
- **Regular Meetings:** Hold weekly check-ins to track progress, identify blockers, and reassign tasks as necessary. Encourage open communication and collaboration.
- **Backup Data:** Maintain offsite or cloud backups of critical raw and processed data to prevent data loss.
- **Ethical & Responsible Research:** Ensure compliance with Institutional Review Board (IRB) or data privacy requirements for EEG research. Handle all data ethically and responsibly.
- **Reproducibility:** Strive for reproducible research by using scripts for all analyses, maintaining clear documentation, and sharing all necessary resources within the repository.

---

## Final Notes

- **Flexibility:** This schedule serves as a comprehensive template but can be adjusted based on student availability, dataset complexity, and conference deadlines. Be prepared to adapt timelines and tasks as needed.
- **Communication:** Maintain consistent communication through weekly meetings, clear GitHub issues, and a running task list to ensure all team members stay on track and understand expectations.
- **Encourage Initiative:** Allow students to take on additional exploratory tasks if they show aptitude or interest in advanced methods (e.g., deep learning, advanced signal processing). Foster an environment of learning and growth.
- **Collaboration Tools:** Utilize GitHub effectively by organizing code, using branches for feature development, and leveraging GitHub Issues or Projects for task management.

With this structured plan, our teams will collaboratively progress from foundational understanding to data exploration, feature extraction, modeling, and finally, manuscript preparation and submission. Let’s work together to achieve a successful publication!

---

**Good luck to everyone involved!**
