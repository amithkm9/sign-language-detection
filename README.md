# Sign Language Translator

A computer vision application that translates sign language gestures into text and speech in real-time.

![Sign Language Translator Demo](demo-screenshot.png)

## Overview

This project uses computer vision and machine learning to recognize American Sign Language (ASL) alphabet signs, numbers, and special characters. It processes webcam input to detect hand gestures and translates them into text and speech, making communication more accessible for the deaf and hard of hearing community.

## Features

- **Real-time sign language detection** using webcam input
- Recognizes **all 26 alphabet letters (A-Z)**, **numbers (0-9)**, space, and period
- **Text-to-speech** conversion of recognized signs
- User-friendly GUI with visual feedback
- Ability to form words and sentences through sequential gesture recognition
- Pause/resume functionality for better control
- Gesture stabilization algorithm to prevent false detections

## Requirements

- Python 3.6+
- OpenCV
- MediaPipe
- scikit-learn
- pyttsx3
- Tkinter
- NumPy
- Pillow

## Installation

1. Clone the repository:
   ```
   git clone https://github.com/yourusername/sign-language-translator.git
   cd sign-language-translator
   ```

2. Install required packages:
   ```
   pip install opencv-python mediapipe scikit-learn pyttsx3 pillow
   ```

## Usage

### Option 1: Running the Application

To use the pre-trained model and start the application immediately:

```
python main.py
```

### Option 2: Training Your Own Model

If you want to create and train your own model:

1. Collect training data:
   ```
   python collect_images.py
   ```
   This will activate your webcam and guide you through capturing images for each sign.

2. Create the dataset from collected images:
   ```
   python create_dataset.py
   ```

3. Train the classifier:
   ```
   python train_classifier.py
   ```

4. Run the application with your custom model:
   ```
   python main.py
   ```

## Using Google Colab (Alternative)

If you want to train the model using Google Colab:

1. Open the provided `Sign_Language_Translator.ipynb` in Google Colab
2. Follow the step-by-step instructions in the notebook
3. Download the trained model
4. Place the model file in your local project directory
5. Run the application locally

## Application Controls

- **Reset Sentence**: Clears the current word and sentence
- **Pause/Play**: Temporarily stops gesture recognition
- **Speak Sentence**: Reads out the current sentence using text-to-speech

## Project Structure

- `collect_images.py`: Script to collect training images using webcam
- `create_dataset.py`: Processes images to extract hand landmarks and create the dataset
- `train_classifier.py`: Trains the Random Forest classifier
- `main.py`: Main application script with GUI and real-time translation
- `model.p`: Pre-trained model file
- `data/`: Directory containing training images
- `data.pickle`: Processed dataset file

## How It Works

1. **Hand Detection**: MediaPipe is used to detect hand landmarks in webcam frames
2. **Feature Extraction**: 21 hand landmarks are normalized and converted to 42 features
3. **Classification**: A Random Forest classifier predicts the sign based on extracted features
4. **Stabilization**: A buffering system ensures that predictions are stable before registering
5. **Word/Sentence Formation**: Characters are combined to form words and sentences
6. **Text-to-Speech**: The pyttsx3 library converts text to audio output

## Customization

- Modify `labels_dict` in `main.py` to change the mapping between class indices and characters
- Adjust `registration_delay` to change how long each sign must be held to be recognized
- Change `stabilization_buffer` size to make recognition more or less sensitive

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## Acknowledgments

- MediaPipe for the hand landmark detection technology
- OpenCV community for computer vision tools
- scikit-learn team for machine learning capabilities

