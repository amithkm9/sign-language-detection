🖐️ Sign Language Detection Using Custom Dataset

This project implements real-time sign language recognition, utilizing a custom dataset to train a robust and accurate gesture recognition model. By converting sign language into text, the project aims to assist in bridging communication gaps.

🚀 Features

1. Custom Dataset: Designed and collected a unique dataset for model training to improve accuracy.

2. Real-Time Gesture Recognition: Leverages Mediapipe and TensorFlow for real-time hand tracking and gesture recognition.

3. Model Training: Includes scripts and data to train custom models tailored to specific sign languages.

4. Scalable Design: Ready for integration into mobile and web-based applications.

📂 Project Structure

1. notebooks/: Contains Jupyter notebooks for data preprocessing, model training, and evaluation.

2. models/: Includes pre-trained models such as action.h5.

3. data/: Stores custom dataset files, including .npy formats for training and validation.

4. scripts/: Python scripts for inference and deployment.

5. README.MD: This documentation.

🛠️ Tools and Technologies

1. Libraries: Mediapipe, TensorFlow, OpenCV, NumPy.

2. Framework: Python (Jupyter Notebook for experimentation).

3. Model Format: The H5 model was trained using the custom dataset.

🎯 Use Cases

1. Translating real-time gestures into text for communication aids.

2. Educational tools for learning and practicing sign language.

3. Assistive devices for individuals with speech or hearing impairments.

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

1. Ensure the data/ folder contains the .npy dataset files.

2. The models/ folder includes the pre-trained action.h5 model.

3. Launch the notebook or run the Python scripts for inference.

🎯 Future Enhancements

1. Expanding the dataset for more comprehensive gesture coverage.

2. Implementing multilingual translation support.

3. Optimizing the model for mobile deployment.

📄 License

This project is licensed under the MIT License. See the LICENSE file for details.


ScreenShots

<img width="659" alt="Screenshot 2025-01-03 at 1 24 34 PM" src="https://github.com/user-attachments/assets/ba78d4f7-ea82-4615-a405-a6e869819205" />
<img width="698" alt="Screenshot 2025-01-03 at 1 24 51 PM" src="https://github.com/user-attachments/assets/610392da-5b02-42ec-8f28-fc7f5daa9b71" />

<img width="710" alt="Screenshot 2025-01-03 at 1 25 00 PM" src="https://github.com/user-attachments/assets/63c23e50-08fa-48a6-8ebe-8c001ca5cfb2" />
<img width="745" alt="Screenshot 2025-01-03 at 1 25 06 PM" src="https://github.com/user-attachments/assets/4b79e590-facf-4a64-8ef7-839a45388d60" />
<img width="772" alt="Screenshot 2025-01-03 at 1 25 15 PM" src="https://github.com/user-attachments/assets/aec0cfed-8d95-431b-a6c6-8239e71687f8" />


