# Class-Agnostic Semantic Edge Detection with U-Net and Weighted BCE Loss

![image](https://github.com/user-attachments/assets/5d7cbe8c-4ec3-4829-9ada-6d6116bcbdc1)


A deep learning project that performs class-agnostic edge detection using a U-Net architecture on the PASCAL VOC 2012 dataset. The model classifies image pixels as either edge or non-edge, leveraging the "void" label (255) in the dataset as a proxy for semantic boundaries. To counter class imbalance, the training uses a Weighted Binary Cross Entropy (BCE) Loss.

🧠 Project Motivation

Semantic edges are crucial for segmentation but often underrepresented in datasets. In PASCAL VOC, many semantic boundaries are marked with the "void" label. This project uses those labels to build a binary edge classifier using U-Net, addressing the imbalance with a weighted BCE loss function.

📦 Features

- U-Net architecture for semantic edge detection.

- Weighted BCE loss to address class imbalance.

- Dynamic batch padding for efficient GPU memory use.

- Mean Intersection over Union (MIoU) as the evaluation metric.

- Train/test comparison of weighted vs. unweighted loss.

- Visualization of model predictions.
