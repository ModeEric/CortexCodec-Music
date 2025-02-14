# Week 1: Getting Started – Setup, Data Familiarization, and Initial Exploration: 2/14/25-2/21/25

Welcome to Week 1 of the CortexCodec Research Projects! This week, our primary goal is to establish a solid foundation by setting up the development environment, gaining hands-on experience with the dataset, and outlining clear, actionable steps for initial analyses. Follow the tasks below, which have been designed to be specific and actionable.

---

## Common Tasks Everyone Must do

1. **Project Environment Setup:**
   - **Clone the Repository & Install Dependencies:**
     - Clone the CortexCodec repository:  
       ```bash
       git clone https://github.com/your_org/CortexCodec.git
       ```
     - Create a Python virtual environment (e.g., using Conda):
       ```bash
       conda create -n cortexcodec python=3.9
       conda activate cortexcodec
       ```
     - Install required packages using the provided `requirements.txt`:
       ```bash
       pip install -r requirements.txt
       ```
   - **Update Documentation:**
     - If you are a new member (or looking for new people to work with), say hi on the #introductions channel


2. **Dataset Familiarization:**
   - **Review Dataset Documentation:**
     - Download and read the OpenNeuro Dataset ds002720 (v1.0.1) documentation PDF or online resource.
     - Be prepared to discuss the details!
    
   ## Detailed tasks that go above the standard

   - **Explore the BIDS Folder Structure:**
     - Open the dataset directory and navigate to a sample participant folder (e.g., `sub-01`).
     - Locate the EEG data files (e.g., files with extensions `.edf` or `.set`).
     - Create a text file (`BIDS_structure.txt`) that lists the folder hierarchy and describes the purpose of each folder (e.g., `/sub-01/eeg/` contains the raw EEG recordings).
   - **Data Loading & Visualization:**
     - Write a Python script or Jupyter Notebook to load one 20-second EEG recording from `sub-01`.
     - Use MNE (or another library) to plot the EEG signals:
       ```python
       import mne
       raw = mne.io.read_raw_edf('path_to_eeg_file.edf', preload=True)
       raw.plot(duration=20, n_channels=10)
       ```
     - Save the resulting plot as `raw_eeg_plot.png` and document any observations (e.g., signal quality, notable artifacts) in your notebook. DM cool plots to Eric or Sid for proof of completion!

3. **Initial Literature & Concept Review:**
   - **Research Review:**
     - Identify and download at least two key research articles on EEG markers for engagement and auditory processing.
     - Write a 300-word summary in a document called `Literature_Review.docx` or a Markdown file `Literature_Review.md`, highlighting the main findings and methods used in the papers.
   



## Project 1 Tasks: Predicting Engagement from EEG Signals (Can be split between people)

1. **Identify Engagement Metrics:**
   - **Task:** Create a table listing at least three candidate EEG markers (e.g., power spectral densities, event-related potentials, phase synchronization measures) and describe how each might relate to listener engagement.
   - **Action:** For each metric, include a short description and one reference from the literature.

2. **Baseline Data Processing:**
   - **Task:** Develop a Python script (`baseline_feature_extraction.py`) that:
     - Reads an EEG file.
     - Computes the mean and variance for each EEG channel.
     - Saves the output in a CSV file (`basic_stats.csv`).
   - **Action:** Run your script on the sample file and inspect the CSV to confirm the results.

3. **Outline Initial Model Ideas:**
   - **Task:** Draw a simple flowchart using a tool like draw.io or even on paper (then scan it) outlining the steps from raw EEG data to engagement prediction.
   - **Action:** Save this diagram as `Project1_Model_Flowchart.png` and add a brief description in `Project_Goals.md`.

---

## Project 2 Tasks: Decoding Musical Content from EEG Signals (Can be split between people)

1. **Mapping Musical Features:**
   - **Task:** Create a list that includes at least three musical elements (e.g., melody, rhythm, harmony).
   - **Action:** For each element, provide one example of an EEG analysis technique that might reveal its neural correlates.

2. **Initial Signal Analysis:**
   - **Task:** Write a Jupyter Notebook (`time_frequency_analysis.ipynb`) to perform a Short-Time Fourier Transform (STFT) on a selected 20-second EEG clip.
   - **Action:** Plot and save the spectrogram (as `spectrogram.png`) and annotate any observed patterns that might correspond to musical elements.

3. **Framework Outline for Predictive Modeling:**
   - **Task:** In a new file, draft a plan that outlines:
     - Data preprocessing steps.
     - Feature extraction techniques.
     - Potential machine learning models to decode the musical content.
   - **Action:** Ensure your plan includes a step-by-step process with at least five numbered steps.

---

## Project 3 Tasks: Comparative Analysis of Models (Can be split between people)

1. **Review Feature Engineering vs. End-to-End Approaches:**
   - **Task:** Write a comparative summary detailing the advantages and disadvantages of:
     - Engineered EEG features (e.g., band power, connectivity metrics).
     - Raw EEG data modeling using deep learning.
   - **Action:** Include references for each approach.

2. **Implement Baseline Pipelines:**
   - **Task:** Create two separate scripts:
     - `engineered_pipeline.py`: Extract a simple set of features (e.g., band power in alpha and beta bands) from the EEG file.
     - `raw_pipeline.py`: Load and preprocess the raw EEG data (e.g., normalization, segmentation) without additional feature engineering.
   - **Action:** Run both scripts on a sample file and document the output shapes and any initial observations in a Markdown file (`Pipeline_Comparison.md`).

3. **Plan for Comparative Metrics and Visualization:**
   - **Task:** In `Project3_Comparative_Analysis.md`, list at least three metrics (e.g., classification accuracy, confusion matrix analysis, t-SNE visualization) you will use to compare the outputs of the two pipelines.
   - **Action:** For each metric, write a brief description of how it will help evaluate the models’ performance and capture the underlying neural representations.

---

This week is focused on preparation and ensuring that every team member has clear, actionable steps to start exploring the dataset and planning their analyses. If you encounter any issues or have questions about the tasks, please reach out to Sid or Eric

Happy coding and exploring!
