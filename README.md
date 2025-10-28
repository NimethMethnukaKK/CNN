[Jute_Pest_Readme.md](https://github.com/user-attachments/files/23189903/Jute_Pest_Readme.md)

# Jute Pest Classification

## Overview
This project is focused on building a **Convolutional Neural Network (CNN)** model to classify images of **jute pests**.  
The goal is to automatically identify 17 types of pests affecting jute crops, which can help in pest monitoring and crop management.

## Dataset
The dataset is organized into three main folders:

- `train/` — images used to train the model  
- `val/` — images used to validate the model during training  
- `test/` — images used to evaluate the model performance  

Each folder contains subfolders corresponding to the 17 pest classes, such as:

- Jute Aphid  
- Jute Semilooper  
- Yellow Mite  
- Jute Stem Girdler  
- Pod Borer  
- Black Hairy  
- Jute Red Mite  
- Field Cricket  
- Scopula Emissaria  
- Termite odontotermes (Rambur)  
- Jute Hairy  
- Mealybug  
- Jute Stem Weevil  
- Termite  
- Cutworm  
- Leaf Beetle  
- Beet Armyworm  

**Note:** The dataset was downloaded from a Google Drive link and preprocessed for this project.

## Features
- Image preprocessing and data augmentation (rotation, zoom, shift, shear, flip, brightness adjustments)  
- CNN built from scratch without transfer learning  
- 17-class classification  
- Evaluation using accuracy, confusion matrix, and classification report  

## Requirements
- Python 3.x  
- TensorFlow / Keras  
- NumPy, Pandas, Matplotlib  
- Scikit-learn  

Install dependencies using:

```bash
pip install tensorflow keras numpy pandas matplotlib scikit-learn
```

## Usage
1. Clone the repository:

```bash
git clone https://github.com/<your-username>/<your-repo>.git
```

2. Upload the dataset or download it from the provided Google Drive link.  
3. Open `jute_pest.ipynb` in **Google Colab** or **Jupyter Notebook**.  
4. Run the notebook cells to:
   - Load and preprocess the dataset  
   - Define the CNN model  
   - Train the model  
   - Evaluate performance on the test set  

## Project Structure
```
├── README.md                 # Project description
├── jute_pest.ipynb           # Colab notebook with code
├── jute_pest_dataset/        # Dataset folder
│   ├── train/                # Training images (17 classes)
│   ├── val/                  # Validation images (17 classes)
│   └── test/                 # Test images (17 classes)
```

## CNN Architecture (Summary)
- **Input:** 128x128 RGB images  
- **Convolutional Layers:** Two Conv2D + MaxPooling blocks  
- **Batch Normalization** after each Conv layer  
- **Fully Connected Layer:** Dense(128) with L2 regularization  
- **Dropout:** 0.5 to prevent overfitting  
- **Output Layer:** Dense(17) with softmax activation  

## Evaluation
- **Metrics:** Accuracy, Confusion Matrix, Classification Report  
- Model performance is evaluated on the **test dataset**.  

## Author
**Your Name**  
Email: your_email@example.com  
GitHub: [https://github.com/<your-username>](https://github.com/<your-username>)

## License
This project is intended for **educational purposes**.
