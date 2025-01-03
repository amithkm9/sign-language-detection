🖐️ Sign Language Detection Using Custom Dataset

This project implements real-time sign language recognition, utilizing a custom dataset to train a robust and accurate gesture recognition model. By converting sign language into text, the project aims to assist in bridging communication gaps.

🚀 Features

Custom Dataset: Designed and collected a unique dataset for model training to improve accuracy.

Real-Time Gesture Recognition: Leverages Mediapipe and TensorFlow for real-time hand tracking and gesture recognition.

Model Training: Includes scripts and data to train custom models tailored to specific sign languages.

Scalable Design: Ready for integration into mobile and web-based applications.

📂 Project Structure
notebooks/: Contains Jupyter notebooks for data preprocessing, model training, and evaluation.

models/: Includes pre-trained models such as action.h5.

data/: Stores custom dataset files, including .npy formats for training and validation.

scripts/: Python scripts for inference and deployment.

README.md: This documentation.

🛠️ Tools and Technologies

Libraries: Mediapipe, TensorFlow, OpenCV, NumPy.

Framework: Python (Jupyter Notebook for experimentation).

Model Format: The H5 model was trained using the custom dataset.

🎯 Use Cases

Translating real-time gestures into text for communication aids.

Educational tools for learning and practicing sign language.

Assistive devices for individuals with speech or hearing impairments.

🌐 How to Run

Clone the repository:
```
bash
Copy code
git clone https://github.com/amithkm9/sign-language-detection.git
```
Install dependencies:
```
bash
Copy code
pip install -r requirements.txt
```

Prepare your environment:

Ensure the data/ folder contains the .npy dataset files.

The models/ folder includes the pre-trained action.h5 model.

Launch the notebook or run the Python scripts for inference.

🎯 Future Enhancements

Expanding the dataset for more comprehensive gesture coverage.

Implementing multilingual translation support.



Optimizing the model for mobile deployment.

📄 License

This project is licensed under the MIT License. See the LICENSE file for details.

ScreenShots

<img width="659" alt="Screenshot 2025-01-03 at 1 24 34 PM" src="https://github.com/user-attachments/assets/ba78d4f7-ea82-4615-a405-a6e869819205" />
<img width="698" alt="Screenshot 2025-01-03 at 1 24 51 PM" src="https://github.com/user-attachments/assets/610392da-5b02-42ec-8f28-fc7f5daa9b71" />

<img width="710" alt="Screenshot 2025-01-03 at 1 25 00 PM" src="https://github.com/user-attachments/assets/63c23e50-08fa-48a6-8ebe-8c001ca5cfb2" />
<img width="745" alt="Screenshot 2025-01-03 at 1 25 06 PM" src="https://github.com/user-attachments/assets/4b79e590-facf-4a64-8ef7-839a45388d60" />
<img width="772" alt="Screenshot 2025-01-03 at 1 25 15 PM" src="https://github.com/user-attachments/assets/aec0cfed-8d95-431b-a6c6-8239e71687f8" />


