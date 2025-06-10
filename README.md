
# SELECTED_TOPICS_Project

### 1️⃣ Setup and Data Import
- Load data from `.zip`
- Parse annotation file without extracting the 9GB file 
- Extract file names and labels
- Optionally extract to disk to speed up I/O

### 2️⃣ Preprocessing and Feature Extraction
- **Mel spectrograms**, STFT and/or MFCC and/or GFCC
- Mono/stereo selection: does spatial information help?
- Spatial features: inter-channel delay, energy difference
- Normalization and padding
- Robustness to background noise and overlapping events

### 3️⃣ Data Augmentation *(to avoid degrading the dataset)* 
- Time stretching
- Pitch shifting
- Add noise (SNR)

### 4️⃣ Dataset Splitting
- Train / Validation / Test split (e.g. 70/15/15 or 60/20/20)

### 5️⃣ Modeling  
(*REFERENCE: VGGNet, ResNet, SqueezeNet, MobileNetMini to capture motion*)
- **Baseline**: 2D CNN  
- **Alternatives**:
  - MLP (on aggregated features)  
  - 1D CNN (on MFCC or waveform)  
  - Hybrid (CNN + RNN)

### 6️⃣ Training and Optimization
- Optimization with Adam, Dropout, EarlyStopping
- Visualization with TensorBoard or matplotlib

### 7️⃣ Evaluation and Analysis
- Confusion matrix
- Accuracy, Precision, Recall, F1-Score
- Effects of noise and augmentation

### 8️⃣ Perform error analysis to identify possible improvements
