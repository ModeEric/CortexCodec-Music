# Week 2: Enhanced Exploration, Preprocessing, and Initial Modeling: 2/21/25-2/28/25

Welcome to Week 2 of the CortexCodec Research Projects! This week, we will build on our initial setup and familiarization work from Week 1 by diving deeper into exploratory data analysis (EDA), refining our preprocessing pipelines, and beginning to implement initial model prototypes. Follow the tasks below, which have been designed to be specific and actionable.

---

## Common Tasks Everyone Must Do

1. **Advanced Data Exploration & Preprocessing:**
   - **Enhanced EDA:**
     - Extend your Week 1 notebooks to include comprehensive statistical summaries (e.g., skewness, kurtosis) and visualize channel-wise distributions using boxplots and violin plots.
     - Investigate potential artifacts and noise in the EEG recordings. Document your findings in a shared EDA report (`EDA_Report.md`).
   - **Preprocessing Improvements:**
     - Experiment with common EEG preprocessing techniques such as band-pass filtering (e.g., 1–40 Hz) and notch filtering to remove line noise.
     - Update your data loading scripts to include these preprocessing steps and validate that the resulting signals show improved quality.
   
2. **Dataset Organization & Documentation:**
   - **Organize Preprocessed Data:**
     - Create a new directory `preprocessed/` in the dataset folder where all filtered and cleaned EEG data will be stored.
     - Write a brief summary (`Preprocessing_Steps.md`) explaining the filters and techniques applied, including references to relevant literature.
   
3. **Team Check-In:**
   - **Project Update:**
     - Post an update in the #project-updates channel summarizing your Week 1 outcomes and outlining your plans for Week 2.
     - Highlight any challenges or insights discovered so far and coordinate next steps with your teammates.

---

## Project 1 Tasks: Predicting Engagement from EEG Signals

1. **Refine Engagement Feature Extraction:**
   - **Task:** Expand your existing feature extraction script (`baseline_feature_extraction.py`) to compute additional engagement-related metrics (e.g., band power in theta, alpha, and beta bands).
   - **Action:** Save the expanded feature set into a new CSV file (`engagement_features.csv`) and update your documentation in `Project1_Feature_Extraction.md`.

2. **Initial Engagement Model Prototype:**
   - **Task:** Develop a simple regression or classification model (e.g., logistic regression, SVM, or a shallow neural network) to predict engagement scores using the engineered features.
   - **Action:** Create a Jupyter Notebook (`engagement_model_prototype.ipynb`) where you:
     - Split the data into training and test sets.
     - Train the model and evaluate its performance using metrics such as accuracy or mean squared error.
     - Document initial performance observations and potential areas for improvement.

3. **Visualization of Engagement Predictions:**
   - **Task:** Plot the predicted versus actual engagement values (or probabilities) and perform an error analysis.
   - **Action:** Save your plots as `engagement_predictions.png` and include a brief discussion of your findings in the notebook.

---

## Project 2 Tasks: Decoding Musical Content from EEG Signals

1. **Enhance Musical Feature Mapping:**
   - **Task:** Refine your list of musical elements (e.g., melody, rhythm, harmony) and associated EEG analysis techniques by including additional details and examples (e.g., the relation of delta waves to slow rhythmic patterns).
   - **Action:** Update your document (`Musical_Feature_Mapping.md`) with these enhancements and add relevant references.

2. **Deep Dive into Time-Frequency Analysis:**
   - **Task:** Improve your initial Short-Time Fourier Transform (STFT) analysis by experimenting with different window sizes and overlap parameters. Consider using wavelet transforms for a multi-resolution analysis.
   - **Action:** Update your notebook (`time_frequency_analysis.ipynb`) with these experiments. Save the updated spectrogram as `refined_spectrogram.png` and annotate any patterns or observations that might correspond to musical elements.

3. **Detailed Predictive Modeling Plan for Musical Content:**
   - **Task:** Draft a more detailed plan for decoding musical content from EEG signals.
   - **Action:** In a new document (`Project2_Modeling_Plan.md`), outline:
     - Advanced data preprocessing steps.
     - Enhanced feature extraction techniques.
     - Proposed model architectures and training strategies.
     - A timeline with at least five numbered steps for incremental development and evaluation.

---

## Project 3 Tasks: Comparative Analysis of Models

1. **Deepen the Comparative Review:**
   - **Task:** Expand your summary comparing engineered EEG features vs. raw EEG data models.
   - **Action:** Update your document (`Comparative_Approaches.md`) to include a discussion on the impact of preprocessing on model interpretability and performance, along with additional references.

2. **Refine Baseline Pipelines:**
   - **Task:** Enhance your two pipelines:
     - **Engineered Pipeline:** Incorporate additional features (e.g., connectivity metrics, spectral entropy) into your engineered feature extraction.
     - **Raw Pipeline:** Experiment with data augmentation strategies and further normalization methods for the raw EEG data.
   - **Action:** Update `engineered_pipeline.py` and `raw_pipeline.py` accordingly. Run both scripts on a sample file and document the output shapes, processing times, and differences in feature distributions in `Pipeline_Comparison.md`.

3. **Visualization of Latent Representations:**
   - **Task:** Begin exploring the latent spaces of both models using dimensionality reduction techniques such as t-SNE or UMAP.
   - **Action:** Create a new notebook (`latent_space_visualization.ipynb`) to visualize and compare the feature spaces. Save the resulting plots as `latent_space_comparison.png` and include a brief discussion on the similarities and differences observed.

---

This week is focused on refining our data processing and starting to implement initial modeling techniques. Please ensure that all code, plots, and documentation are updated in the repository. If you encounter any issues or have questions about the tasks, please reach out to Sid or Eric.

Happy coding and exploring!
