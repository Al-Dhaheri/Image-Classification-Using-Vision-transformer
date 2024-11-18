# Image Classification Using Vision Transformer

This project demonstrates the use of Vision Transformer (ViT) for image classification from scratch. The main focus is on classifying surface defects in metal, using the public **NEU Metal Surface Defects Dataset**. The model was trained to identify and classify different defect types present on the metal surfaces. The training was conducted in both **Google Colab** and **Jupyter Notebook**, allowing flexibility for different computational environments.

## Dataset: NEU Metal Surface Defects Data
- The dataset used in this project is the **NEU Metal Surface Defects Dataset**, which consists of images representing six types of surface defects found in steel surfaces: **Crazing, Inclusion, Patches, Pitted Surface, Rolled-in Scale, and Scratches**.
- Each image is labeled with the type of defect it contains, which allows us to train a model to automatically classify these defects.

## Model: Vision Transformer (ViT)
- The model used for this project is a **Vision Transformer (ViT)**, trained from scratch. ViT is known for its ability to perform well on image recognition tasks by treating image patches similarly to sequences in NLP tasks, using **attention mechanisms**.
- The model was trained using **PyTorch**, with optimization using the **Adam** optimizer.
- The training process used **data augmentation** techniques to improve generalization and reduce overfitting, such as random cropping, horizontal flipping, and color jittering.

## Results
- The model was able to achieve a decent level of accuracy on the test set. Below are some visual examples showing how well the model was able to classify metal surface defects.
- Examples of model predictions:
  - The images below show true labels versus predicted labels for various samples from the test set.

Classification Results - Set 1
![download (2)](https://github.com/user-attachments/assets/1ca33c3c-7f4d-4a98-bf53-5339ce061497)

Classification Results - Set 2
![download (1)](https://github.com/user-attachments/assets/cbecb1a1-2aeb-42f8-b925-e28c9df6d44d)

The model was trained to identify six different types of metal surface defects and was able to distinguish between them with an average accuracy of **78%**. The **ROC curve** also demonstrates the performance of the model across different classes.

## How to Use This Repository

### Running on Google Colab
1. **Clone the repository**:
   ```
   !git clone https://github.com/Al-Dhaheri/Image-Classification-Using-Vision-transformer
   ```
2. **Upload the dataset to Google Drive** or provide a path to access it directly.
3. **Run the Colab notebook** (`image_classifier_colab.ipynb`) by mounting Google Drive to access the required files.
   - Make sure to modify paths if needed to access your dataset and save the model.

### Running Locally Using Jupyter Notebook
1. **Clone the repository**:
   ```
   git clone https://github.com/Al-Dhaheri/Image-Classification-Using-Vision-transformer
   ```
2. **Make sure to Install dependencies**:

3. **Run the Jupyter notebook** (`image_classifier_from_scratch.ipynb`) on your local environment.
   - Ensure that the dataset path is correctly set in the notebook.

## Project Highlights
- **Dataset**: NEU Metal Surface Defects Dataset containing six classes of metal defects.
- **Model**: Vision Transformer trained from scratch using PyTorch.
- **Environments**: Flexible training on both Google Colab and local Jupyter Notebook.
- **Results**: Achieved approximately 78% accuracy, with a notable capability of distinguishing most defect types, visualized with classification examples.

## Examples of Classification Results
- Here are some of the classification results of the model on test images:

Classification Results - Set 1
![download (2)](https://github.com/user-attachments/assets/1ca33c3c-7f4d-4a98-bf53-5339ce061497)

Classification Results - Set 2
![download (1)](https://github.com/user-attachments/assets/cbecb1a1-2aeb-42f8-b925-e28c9df6d44d)

## Future Improvements
- **Object Detection**: Incorporate object detection models to not only classify but also localize defects using bounding boxes.
- **Data Augmentation**: Apply advanced augmentation techniques specific to the challenging classes to improve recall.
- **Fine-Tuning**: Use a pre-trained Vision Transformer model and fine-tune it on the metal defect dataset to improve accuracy further.

## Conclusion
The Vision Transformer model effectively demonstrates the potential to classify different metal surface defects. The project is a good starting point for exploring how transformer-based models can be utilized in defect detection tasks in industrial settings.
