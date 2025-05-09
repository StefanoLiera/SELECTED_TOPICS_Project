# SELECTED_TOPICS_Project




### 1️⃣ Setup e Importazione dati
-  Caricamento dati da `.zip`
-  Parsing file annotazione (`idmt_traffic_all.txt`)
-  Estrazione nomi file + etichette
-  Eventuale estrazione su disco per velocizzare I/O

### 2️⃣ Preprocessing e Feature Extraction
-  **Mel spectrogrammi** and STFT and/or MFCC and/or GFCC
-  Scelta mono/stereo: does spatial information help? 
-  Spatial features: inter-channel delay, energy difference
-  Normalizzazione e padding
-  Robustness to background noise and overlapping events


### 3️⃣ Data Augmentation *(to not degrade the dataset)
-  Time stretching
-  Pitch shifting
-  Aggiunta rumore (SNR)
-  Convoluzione con impulse responses

### 4️⃣ Divisione dataset
-  Train / Validation / Test split (es. 70/15/15) or (es. 60/20/20)

### 5️⃣ Modellazione 
(DE REF: VGGNet, ResNet, SqueezeNet, MobileNetMini to capture the movement)
-  **Baseline**: CNN 2D 
-  **Alternative**:
  - MLP (su feature aggregate)
  - CNN 1D (su MFCC o waveform)
  - Hybrid (CNN + RNN)

### 6️⃣ Training e Ottimizzazione
-  Ottimizzazione con Adam, Dropout, EarlyStopping
-  Visualizzazione con TensorBoard o matplotlib

### 7️⃣ Valutazione e Analisi
-  Confusion matrix
-  Accuracy, Precision, Recall, F1-Score
-  Effetti del rumore e delle augmentationi
