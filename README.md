# 🦵 Osteoarthritis Multiclass Classification

## 📌 Project Overview
This project aims to classify the severity of knee osteoarthritis from X-ray images. It compares the performance of two different Convolutional Neural Network (CNN) architectures, AlexNet and EfficientNetB0, to determine which model is more effective for this task.

## 📊 Dataset
The dataset contains knee X-ray images categorized into five classes representing different stages of osteoarthritis: **Doubtful, Mild, Moderate, Normal, and Severe**. The training dataset includes 5375 images, while the validation and test sets contain 806 and 586 images, respectively. All images have a consistent resolution of 224x224 pixels and a 1:1 aspect ratio.

## 🔍 Key Findings
1. **Data consistency**: All images in the dataset share a uniform resolution of 224x224 pixels and a 1:1 aspect ratio.
2.**Color distribution**: The color histograms show a symmetrical, bell-shaped distribution, with most pixel intensity values centered around 150. This indicates a consistent level of medium brightness across the images.
3. **Model performance**: The EfficientNetB0 model, even without pretrained weights, outperformed the AlexNet model across all evaluation metrics (accuracy, precision, recall, and F1-score).
4. **Overfitting**: Both models exhibited poor performance, with accuracy hovering around 20%, suggesting they struggled to generalize from the training data and were essentially making random guesses. This indicates a significant issue with the models' ability to learn meaningful patterns from the dataset.

## 📈 Steps
1. **Data Exploration and Analysis (EDA)**: Performed initial analysis on the dataset to understand image characteristics such as color distribution, aspect ratio, and resolution, and to identify potential issues like lighting inconsistencies and noise.
2. **Preprocessing**: All images were resized to 224x224 pixels to ensure uniformity and meet the input requirements of the selected models.
3. **Modeling and Evaluation**: Two separate CNN models, AlexNet and EfficientNetB0, were built and trained on the preprocessed data. Model performance was evaluated using accuracy, precision, recall, and F1-score, along with confusion matrices.
4. **Tuning**: Callbacks for checkpointing, early stopping, and reducing the learning rate were used during training to optimize the models and prevent overfitting.

## 💡 Conclusion
Both the AlexNet and EfficientNetB0 models performed poorly on the task of classifying knee osteoarthritis, with accuracies of only around **20-21%**. This suggests the models were unable to effectively learn and generalize from the provided data. The EfficientNetB0 model did show slightly better performance, but neither model is suitable for practical use without further improvements.

## 🔮 Possible Future Works
1. **Data Augmentation**: Implement data augmentation techniques to increase the diversity of the training data and help the model generalize better.
2. **Transfer Learning**: Utilize pre-trained weights from a model like EfficientNetB0 trained on a large dataset like ImageNet to leverage existing knowledge of image features.
3.**Advanced Architectures**: Experiment with more advanced and larger models to improve feature extraction capabilities.

## 👨‍💻 Author
**Liliana Djaja Witama** | Undergraduate Data Science Student at BINUS University
