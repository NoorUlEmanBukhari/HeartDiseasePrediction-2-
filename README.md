# Image Classification with CNN and Image Augmentation

##  Project Overview
This project builds a Convolutional Neural Network (CNN) to classify images into two categories.  
We used **Image Augmentation** to artificially increase the size of the dataset and improve the model’s generalization.  
The model is trained using Keras with TensorFlow backend.  

---

##  Dataset
- The dataset is divided into:
  - **Training set**: 4438 images (2 classes)
  - **Testing set**: 1114 images (2 classes)
- Images are normalized (scaled between `0 and 1`).

---

##  Libraries Used
- **TensorFlow / Keras** → For building and training the CNN model.  
- **ImageDataGenerator** → For image augmentation (rotation, zoom, flipping).  
- **NumPy** → For numerical computations.  
- **Matplotlib** → For visualization (loss/accuracy plots).

---

##   Image Preprocessing
- All images are resized to **224x224** pixels.  
- Pixel values scaled from **0–255 → 0–1**.  
- Augmentation applied on training images:
  - Rotation: up to 20°  
  - Zoom: up to 20%  
  - Horizontal Flip  

---

##  Model Training
- Data is loaded in **batches of 32**.  
- Model learns over multiple **epochs** (full passes over training data).   

---

##  Flow of the Project
1. Load dataset (train/test).  
2. Apply preprocessing and augmentation using `ImageDataGenerator`.  
3. Create CNN model.  
4. Train model with training data (`train_generator`).  
5. Validate model with test data (`test_generator`).  
6. Evaluate performance (accuracy, loss).  
7. Save trained model for future predictions.  

---

##  Results
- Model outputs **binary classification (0 or 1)** for each image.  
- Training and validation accuracy/loss can be visualized using Matplotlib.  

---

##  How to Run
```bash
# Clone repository
git clone <[your-repo-link](https://github.com/NoorUlEmanBukhari/HeartDiseasePrediction-2-)>

# Install dependencies
pip install tensorflow numpy matplotlib


