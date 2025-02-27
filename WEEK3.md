# Week 3: Full Pipeline Integration & Iterative Refinement  
*Dates: 3/1/25 – 3/8/25*

With an accelerated 12-week timeline, our goal for Week 3 is to integrate our work from Weeks 1 and 2 into a unified, end-to-end pipeline for all three projects. By the end of this week, we should have baseline pipelines that run from raw data ingestion to preliminary model predictions. Once this full pipeline is operational, subsequent weeks will focus on refining each component—ranging from data cleaning to model architecture and hyperparameter tuning.

---

## Overall Goals

- **End-to-End Pipeline:**  
  Develop and test a complete workflow that covers:
  - Data loading and preprocessing (filtering, artifact removal, segmentation)
  - Feature extraction (both engineered and raw data approaches)
  - Initial model training and evaluation for engagement prediction, musical content decoding, and comparative analysis
  
- **Modular & Reproducible:**  
  Ensure that the pipeline is modular so that improvements or modifications (e.g., design choices for cleaning or model processing) can be implemented in isolation and compared easily.

- **Baseline Performance:**  
  Establish baseline metrics for each project to serve as reference points for iterative improvements in subsequent weeks.

---

## Common Tasks for All Projects

1. **Unified Data Loader & Preprocessor:**  
   - Develop a centralized script (`data_pipeline.py`) that:
     - Loads raw EEG data from the preprocessed/ directory.
     - Applies a standardized set of preprocessing steps (band-pass filtering, notch filtering, segmentation).
   - Validate that the output meets quality criteria and is ready for feature extraction or direct model input.

2. **Integration of Feature Extraction:**  
   - Combine the feature extraction scripts from Projects 1 and 3 into the pipeline.
   - Ensure that both engineered features (e.g., band power, connectivity metrics) and raw data flows are supported.
   - Output should be stored in a structured format (e.g., CSV for features and standardized arrays for raw inputs).

3. **Model Training & Evaluation Framework:**  
   - Create a common training module (`model_training.py`) that:
     - Loads preprocessed data and corresponding features.
     - Trains baseline models (e.g., simple regression/classification for engagement; baseline neural network for musical content decoding).
     - Evaluates performance with standardized metrics.
   - Generate summary reports (or plots) comparing predicted vs. actual outputs across tasks.

---

## Project-Specific Tasks

### Project 1: Predicting Engagement from EEG Signals

- **Pipeline Integration:**  
  - Integrate the updated feature extraction script from Week 2 to compute extended engagement metrics.
  - Test the regression/classification model within the unified pipeline.
  - Output: A summary CSV or visualization (e.g., `engagement_pipeline_output.png`) showing baseline performance.

- **Initial Model Comparison:**  
  - Experiment with at least two model types (e.g., logistic regression and shallow neural network) within the pipeline.
  - Document performance metrics and any initial error analyses in `Project1_Pipeline_Evaluation.md`.

### Project 2: Decoding Musical Content from EEG Signals

- **Unified Processing & Analysis:**  
  - Ensure the STFT (and/or wavelet-based) analysis integrates smoothly into the data pipeline.
  - Combine the refined musical feature mapping with the predictive modeling plan.
  - Output: A preliminary prediction report or visualization (e.g., `musical_content_pipeline_output.png`) that correlates EEG features with musical elements.

- **Model Pipeline Integration:**  
  - Implement a baseline model within the pipeline to decode musical content.
  - Validate the approach with a small subset of the dataset and record initial performance indicators.

### Project 3: Comparative Analysis of Models

- **Dual Pipeline Execution:**  
  - Integrate both the engineered features pipeline and the raw data pipeline into the unified framework.
  - Ensure that both pipelines run concurrently with shared preprocessed data.
  - Output: Documented comparisons in `Pipeline_Comparison_Week3.md` that include:
    - Feature distribution summaries
    - Processing times
    - Baseline evaluation metrics for both approaches

- **Latent Space & Visualization:**  
  - Extend the latent space visualization notebook (`latent_space_visualization.ipynb`) to work with the full pipeline outputs.
  - Save updated plots (e.g., `latent_space_comparison_week3.png`) and note any differences between the two approaches.

---

## Additional Development Goals

- **Design Reviews:**  
  - Schedule a team meeting to review pipeline design choices, discuss potential improvements in data cleaning, feature processing, and model architecture.
  
- **Documentation & Code Quality:**  
  - Update all relevant documentation files (e.g., `Project_Goals.md`, `Preprocessing_Steps.md`) to reflect the integrated pipeline.
  - Ensure that code is modular and well-commented for ease of iterative refinement in future weeks.

- **Version Control & Testing:**  
  - Commit and push all updates to the repository.
  - Set up basic unit tests for critical components of the pipeline to ensure reproducibility and facilitate debugging.

---

By the end of Week 3, we should have a fully operational baseline pipeline that serves as the foundation for further enhancements and model refinements. Let’s work collaboratively to integrate, test, and document every component, ensuring our pipeline is robust, modular, and ready for iterative improvement in the coming weeks.
