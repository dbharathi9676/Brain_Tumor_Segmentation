# 🧠 Brain Tumor Segmentation Using U-Net


# 📜 Overview

Brain tumor segmentation is a crucial task in medical imaging to assist in early diagnosis and treatment planning. This project implements a *U-Net-based deep learning model* to perform *accurate segmentation* of brain tumors from MRI images. The U-Net architecture ensures precise pixel-level predictions, even with limited data.

The goal is to Develop a U-Net model incorporating Batch Normalization, Layer Normalization, and Group Normalization. Train each version on a brain MRI dataset and use IoU loss and Dice loss as metrics. Analyse the results to identify the most effective normalization technique for segmentation accuracy and reliability.
# 🛠 Features

## 1. Data Preprocessing:
- Handled MRI scan images for noise reduction and normalization.
- Resized and augmented images to improve model robustness.

## 2. U-Net Model Implementation:
- Built the *U-Net architecture* for semantic segmentation.
- Trained the model using a dataset of MRI brain scans to identify tumor regions.

## 3. Model Evaluation:
- Evaluated the segmentation accuracy using:
    - *Dice Coefficient*  
    - *IoU (Intersection over Union)*  
  

## 4. Visualization:
- Visualized predictions with segmented masks overlaid on input MRI images.
- Compared ground truth and predicted segmentation for performance evaluation.

## 5. Model Deployment:
- Provided a framework to load the trained model for inference on new MRI images.

# 🔧 Tools and Technologies

- *Programming Language*: Python  
- *Libraries Used*:
    - Data Handling: Pandas, NumPy, OpenCV  
    - Model Building: TensorFlow/Keras  
    - Visualization: Matplotlib, Seaborn  
    - Progress Monitoring: tqdm  

# 🚀 How to Use

1. *Clone the repository*:
   ```bash
   git clone https://github.com/yourusername/brain-tumor-segmentation.git
   cd brain-tumor-segmentation


# 📊 Results
- Batch Normalization exhibited consistent performance across various epochs, maintaining high accuracy and respectable IoU and Dice scores. It showed good generalization capabilities, making it a reliable choice for brain tumor segmentation. However, the segmentation precision improved notably with increased epochs, highlighting its dependency on longer training durations.

- Layer Normalization demonstrated adequate performance, with significant improvements observed when the training epochs were increased. Although it slightly lagged behind Batch and Group Normalization in overall metrics, it still provided robust results, particularly in maintaining high accuracy across training, validation, and test sets.
- Group Normalization emerged as the superior normalization strategy in this study. It consistently achieved the highest scores in IoU and Dice metrics, indicating superior segmentation accuracy and precision. This performance was particularly evident at 100 epochs, where Group Normalization outperformed the other techniques, showcasing its effectiveness in handling the complexities of brain tumor segmentation.
- Therefore, Group Normalization is recommended for brain tumor segmentation based on the provided observations, particularly for achieving the highest segmentation accuracy and robustness.




# conclusion
- we tested three normalization techniques—Batch Normalization, Layer Normalization, and Group Normalization—on brain tumor segmentation using deep learning. The performance was measured over 50 and 100 epochs based on factors like accuracy, training loss, and segmentation quality (using metrics like IoU and Dice score).

The results showed that while all three normalization methods worked well, Group Normalization performed the best, delivering the highest accuracy and consistency across different datasets. It was the most reliable technique for brain tumor segmentation.

In short, Group Normalization is the top choice for this task, and future improvements could involve exploring additional techniques like attention mechanisms and combining data from multiple sources to make the segmentation even better.

 # 🔮 Future Scope
- we can apply segmentation  for other body parts like heart , liver, kidney with the help of group 
  Normalization technique and U - Net Architecture.
- Deploy the model as a web app for real-time segmentation using Flask or Streamlit.



