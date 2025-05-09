# SELECTED_TOPICS_Project




### 1️⃣ Setup e Importazione dati
-  Caricamento dati da `.zip`
-  Parsing file annotazione (`idmt_traffic_all.txt`)
-  Estrazione nomi file + etichette
-  Eventuale estrazione su disco per velocizzare I/O

### 2️⃣ Preprocessing e Feature Extraction
-  Conversione a **Mel spectrogrammi**
-  Scelta mono/stereo
-  Normalizzazione e padding
-  Salvataggio spettrogrammi se necessario

### 3️⃣ Data Augmentation *(facoltativo ma consigliato)*
-  Time stretching
-  Pitch shifting
-  Aggiunta rumore (SNR)
-  Convoluzione con impulse responses

### 4️⃣ Divisione dataset
-  Train / Validation / Test split (es. 70/15/15) or (es. 60/20/20)

### 5️⃣ Modellazione
-  **Baseline**: CNN 2D 
-  **Alternative**:
  - MLP (su feature aggregate)
  - CNN 1D (su MFCC o waveform)
  - Hybrid (CNN + RNN)

### 6️⃣ Training e Ottimizzazione
-  Ottimizzazione con Adam, Dropout, EarlyStopping
-  Visualizzazione con TensorBoard o matplotlib

### 7️⃣ Valutazione e Analisi
-  Accuracy + confusion matrix
-  Errori per classe
-  Effetti del rumore e delle augmentationi
