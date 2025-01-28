
---

# Document Classification and Information Extraction System  

This project is a machine learning-based system for classifying and extracting information from different types of identification documents, such as Aadhaar cards, PAN cards, and college ID cards (DTU ID). The system uses a Convolutional Neural Network (CNN) for classification and custom extraction functions for information retrieval.

---

## Features  

- **Document Classification**:  
  Classifies input images into the following categories:  
  - Aadhaar  
  - PAN  
  - DTU ID  

- **Information Extraction**:  
  Extracts details specific to the classified document type, such as Aadhaar number, PAN card details, and college ID information.

- **Deep Learning Model**:  
  - Built with CNN using TensorFlow/Keras.  
  - Data augmentation for better model performance and generalization.  

---

## Installation  

1. **Clone the Repository**:  
   ```bash  
   git clone https://github.com/yourusername/document-classification.git  
   cd document-classification  
   ```  

2. **Install Dependencies**:  
   Install the required Python libraries:  
   ```bash  
   pip install -r requirements.txt  
   ```  

3. **Dataset Setup**:  
   - Organize your dataset in the following structure:  
     ```
     dataset/
     ├── Aadhaar/
     │   ├── image1.jpg
     │   ├── image2.jpg
     ├── PAN/
     │   ├── image1.jpg
     │   ├── image2.jpg
     ├── DTU_ID/
     │   ├── image1.jpg
     │   ├── image2.jpg
     ```

4. **Train the Model**:  
   Run the script to preprocess images and train the model:  
   ```bash  
   python train_model.py  
   ```  

5. **Test the Model**:  
   Use the trained model to predict and extract details from a document:  
   ```bash  
   python predict.py --image-path /path/to/image.jpg  
   ```

---

## Usage  

### 1. **Train the Model**  
   Run the training script to train the CNN:  
   ```bash  
   python train_model.py  
   ```  

### 2. **Classify and Extract Information**  
   Use the trained model to classify a document and extract its information:  
   ```bash  
   python predict.py --image-path /path/to/image.jpg  
   ```  
   Example output:  
   ```
   Predicted Class: Aadhaar  
   Extracted Information:  
   Aadhaar Number: 1990 5512 9932 1875  
   ```

---

## Project Structure  

```
├── dataset/                  # Dataset folder (organized by class labels)  
├── train_model.py            # Script to train the CNN model  
├── predict.py                # Script for document classification and information extraction  
├── model/                    # Folder to save trained models  
├── requirements.txt          # Python dependencies  
├── README.md                 # Project documentation  
```

---

## Dependencies  

- Python 3.x  
- TensorFlow/Keras  
- OpenCV  
- NumPy  
- scikit-learn  
- Matplotlib  

Install all dependencies using:  
```bash  
pip install -r requirements.txt  
```

---

## Example  

**Input Image**:  
Upload an Aadhaar card image.  

**Output**:  
- Predicted Class: Aadhaar  
- Extracted Details:  
  ```
  Aadhaar Number: 1990 5512 9932 1875  
  ```

---

## License  

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

Feel free to customize this based on your project's specifics or style!
