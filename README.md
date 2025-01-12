# 🎵 Speech Emotion Recognition

This project utilizes advanced machine learning techniques to recognize emotions from speech data. The ultimate goal is to develop a robust model capable of identifying emotional tones like happiness, sadness, anger, and fear from audio recordings.

---

## 🚀 Datasets Used

This project leverages the following datasets:
1. **🎭 Crowd-sourced Emotional Multimodal Actors Dataset (Crema-D)**
2. **🎤 Ryerson Audio-Visual Database of Emotional Speech and Song (RAVDESS)**
3. **🎶 Surrey Audio-Visual Expressed Emotion**
4. **🗣️ Toronto Emotional Speech Set**

---

## 🛠️ Project Workflow

1. **🔍 Data Preparation**  
   - Unified four datasets into a single DataFrame containing paths and emotion labels.
   - Used Kaggle API to fetch datasets and unzipped them for processing.

2. **🎚️ Feature Extraction**  
   - Extracted key audio features like MFCC, Chroma, and Mel Spectrogram for training.

3. **🤖 Model Training**  
   - Trained a machine learning model to classify speech data into corresponding emotional categories.

---

## 📂 Dataset Details

### **RAVDESS**
Structured filenames provide metadata for the audio files:
- **Modality:** (01 = full-AV, 02 = video-only, 03 = audio-only)
- **Vocal Channel:** (01 = speech, 02 = song)
- **Emotional Intensity:** (01 = normal, 02 = strong)
- **Statement:** (01 = "Kids are talking by the door", 02 = "Dogs are sitting by the door")
- **Repetition:** (01 = 1st, 02 = 2nd)
- **Actor:** (Odd = male, Even = female)

Example: `02-01-06-01-02-01-12.mp4`  
- Modality: Video-only  
- Vocal Channel: Speech  
- Emotion: Fearful  
- Intensity: Normal  
- Statement: "Dogs"  
- Repetition: 1st  
- Actor: Female

### **Crema-D**
This dataset contains diverse emotional speech audio, integrated into the DataFrame for seamless processing.

---

## 💻 How to Run

1. Clone the repository:
   ```bash
   git clone <repository-link>
   cd speech-emotion-recognition
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Fetch datasets using Kaggle API and unzip into the appropriate directories.

4. Launch the Jupyter Notebook:
   ```bash
   jupyter notebook Speech_Emotion_Recognition.ipynb
   ```

---

## 📈 Results

The model demonstrated high accuracy in classifying emotions across various categories:
- Happiness
- Sadness
- Anger
- Fear
- Neutral

---

## 🧰 Tools and Libraries

- **Python**
- **Librosa**
- **Pandas**
- **Scikit-learn**
- **TensorFlow/Keras**
- **Matplotlib**
- **Seaborn**

---

## 🌟 Future Scope

- Implement real-time emotion recognition from live audio.
- Enhance noise-handling capabilities.
- Extend multilingual support for broader applications.

---

## 📜 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgements

Grateful to the creators of the datasets and open-source libraries that enabled this project.
