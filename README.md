
# Deep Facial Recognition System
![Python](https://img.shields.io/badge/python-3670A0?style=flat&logo=python&logoColor=ffdd54) ![OpenCV](https://img.shields.io/badge/opencv-%23white.svg?style=flat&logo=opencv&logoColor=white)  ![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=flat&logo=TensorFlow&logoColor=white) ![Anaconda](https://img.shields.io/badge/Anaconda-%2344A833.svg?style=flat&logo=anaconda&logoColor=white)
## Description
This project implements a Siamese Neural Network for efficient image triplet analysis, seamlessly integrating OpenCV for image collection. Three categories of images - positive, negative, and anchor - are collected using OpenCV and preprocessed to standardize dimensions to 100x100 pixels in JPEG format.

![Flow Chart](https://github.com/MOHINI1403/Deep-Facial-Recognisation-System/blob/main/collection_images/flow-chart-C-of.png)

### Research Paper
[Link to Research Paper](https://github.com/MOHINI1403/Deep-Facial-Recognisation-System/blob/main/Siamese_Neural_Network.pdf)

## Workflow Overview

1. **Data Collection:** Utilizing OpenCV, 300 images are collected from each category: positive, negative, and anchor.
2. **Preprocessing:** Images are resized to 100x100 pixels and converted to JPEG format.
3. **Dataset Creation:** Positive and negative image pairs are combined with anchor images, generating a labeled dataset. Positive pairs are labeled as 1, and negative pairs as 0.
4. **Training Data Preparation:** The dataset is split into training and testing sets in a 70-30 ratio and batched with a size of 8 for efficient processing.
5. **Siamese Model Architecture:** A Siamese neural network is constructed with an embedding layer for feature extraction and a custom distance layer for similarity computation.
6. **Model Training:** The Siamese model is trained on the prepared dataset, optimizing recall and precision metrics for performance evaluation.
7. **Real-Time Verification:** OpenCV is employed for real-time image verification, showcasing the practical application of the trained model.

### Embedding Layer
![Embedding Layer](https://github.com/MOHINI1403/Deep-Facial-Recognisation-System/blob/main/collection_images/embedding_layer.png)

### Siamese Model
![Siamese Model](https://github.com/MOHINI1403/Deep-Facial-Recognisation-System/blob/main/collection_images/siamese_model.png)

## Tech Stack
### Python
### Tensorflow
### Open-CV

## Usage
1. **Clone the Repository:**
   ```bash
   git clone https://github.com/MOHINI1403/Deep-Facial-Recognisation-System.git
   ```

2. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Folder Structure:**
   - **Data Folder:**
     - Contains three sections: positive, negative, and anchor images.
     - Use OpenCV to collect images for the positive and negative sections.
     - Negative images can be downloaded [here](insert_link_to_download_negative_images).
   - **Application Images Folder:**
     - Contains two folders: input_image and verification_images.
     - verification_images folder should contain around 50 images randomly selected from positive and anchor sets.

4. **Virtual Environment:**
   - Create a virtual environment named faceid:
     ```bash
     python -m venv faceid
     ```
   - Activate the virtual environment:
     - On Windows:
       ```bash
       faceid\Scripts\activate
       ```
     - On macOS and Linux:
       ```bash
       source faceid/bin/activate
       ```

## Contribution
Contributions are welcome! Fork the repository, make your changes, and submit a pull request.

## Key Components
- **OpenCV Integration:** Efficient image collection and real-time verification.
- **Siamese Neural Network:** Architecture for learning image similarity through feature embeddings.
- **Custom Distance Layer:** Calculates the L1 distance between embeddings for similarity assessment.
- **Training Evaluation:** Metrics such as recall and precision used to assess model performance.

### Further Assitance :
Try Reading this Documentation :
![Link to Documentation](upnote://x-callback-url/openNotebook?notebookId=b5e86e92-46f3-4b9b-b719-c6a26790a4c8)


