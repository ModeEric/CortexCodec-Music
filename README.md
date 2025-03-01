# CortexCodec Research Projects

Welcome to the CortexCodec research repository. In this repository, we explore three interconnected research tasks using a shared EEG dataset. Each task leverages EEG data to advance our understanding of the neural correlates of music perception and cognition.

## Common Dataset Information

All projects now utilize the EEG dataset from **ds002722**, originally collected for the Brain-Computer Music Interface for Monitoring and Inducing Affective States (BCMI-MIdAS) study. This dataset comprises recordings from 19 healthy adult participants who listened to 40-second music clips generated in real-time by a synthetic music generator. During each trial, the music was designed to target specific affective states (defined by valence and arousal), with the first 20 seconds corresponding to one target state and the remaining 20 seconds to a second target state. The data, formatted according to the BIDS standard, were recorded at a sampling rate of 1 kHz. For full dataset details, please refer to the [OpenNeuro Dataset ds002722](https://openneuro.org/datasets/ds002722).

---

## Project 1: Predicting Engagement from EEG Signals

### Research Question
**Can we predict the engagement of a listener based solely on their EEG signals?**

### Motivation & Research Directions
Understanding listener engagement is key to personalizing and enhancing experiences in multimedia environments. Engagement levels not only reflect cognitive and emotional states but also have implications for adaptive music systems and therapeutic interventions.

- **Feature Extraction and Signal Analysis:**  
  Identify EEG markers—such as power spectral densities, event-related potentials, and phase synchronization—that correlate with engagement levels.
  
- **Model Development:**  
  Develop machine learning models, ranging from classical statistical methods to deep learning architectures, to predict engagement. Compare the performance of different approaches.

- **Validation and Real-Time Implementation:**  
  Validate the models against subjective ratings and behavioral data. Explore the feasibility of deploying these models in real-time systems to provide adaptive feedback during music listening sessions.

---

## Project 2: Decoding Musical Content from EEG Signals

### Research Question
**Can we predict the song (or musical content) that a listener is exposed to solely based on their EEG signals?**

### Motivation & Research Directions
Decoding musical content from neural signals provides insights into how auditory information is encoded in the brain. Successfully mapping EEG data to musical stimuli could revolutionize the development of brain-computer interfaces for music recommendation and composition.

- **Signal-to-Feature Mapping:**  
  Develop methodologies to extract musical features—such as melody, rhythm, and harmony—from EEG signals.

- **Predictive Modeling:**  
  Construct and train models to infer the musical stimulus from EEG patterns. Evaluate the accuracy of predictions across different genres and musical structures.

- **Neural Encoding Analysis:**  
  Investigate how various musical elements are represented in the EEG data, thereby enhancing our understanding of auditory processing in the brain.

---

## Project 3: Comparative Analysis of Models Trained on Engineered EEG Features vs. Raw EEG Data

### Research Question
**What similarities exist between models trained on engineered EEG features and those trained directly on raw EEG data when performing the same task?**

### Motivation & Research Directions
Comparing different modeling approaches can reveal insights into the underlying neural representations captured by each method. By contrasting models trained on engineered features with those using raw data, we aim to understand the trade-offs between preprocessing and end-to-end learning in neural decoding tasks.

- **Model Architectures:**  
  Develop two parallel pipelines:
  - **Engineered Features Pipeline:** Extract predefined features from the EEG data before model training.
  - **Raw Data Pipeline:** Train models directly on preprocessed raw EEG signals without feature engineering.

- **Performance and Representation Comparison:**  
  Analyze model outputs by examining misclassification patterns, distributions of logits, and latent space representations (using techniques like t-SNE). Determine whether both approaches capture similar neural phenomena.

- **Implications for Model Design:**  
  Use insights from the comparative analysis to refine model architectures, aiming for improved interpretability, robustness, and performance in EEG-based decoding tasks.

---

*The CortexCodec Team*
