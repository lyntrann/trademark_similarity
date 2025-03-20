# Trademark Image Retrieval via Multi-Modal Feature Fusion
February 8, 2022, **Applied Sciences (MDPI)**

DOI: 10.3390/app12031752

Authors: Hayfa Alshowaish, Yousef Al-Ohali, Abeer Al-Nafjan

## 1. Problem: Manual trademark similarity detection is inefficient (subjectivity in judgment, lack of automation)

## 2. Proposed Solution: Use deep learning:

- CNNs (ResNet-50 and VGG-16) extract image features automatically.
- Euclidean distance is used to measure similarity between trademarks.
- The system retrieves the most similar registered trademarks to a given query, reducing the examiner's workload.

## 3. Results:

- Dataset:  Middle East Technical University dataset (METU dataset)
- ResNet-50 outperformed VGG-16 in most tests.
- Best experiment (ResNet-50 + PCA):
  - Average Rank: 67,067.788
  - Normalized Average Rank (NAR): 0.0725 (lower is better)
  - Mean Average Precision (mAP): 0.774 (higher is better)
- Comparison with previous studies:
Previous best method (Tursan et al., 2017): NAR = 0.086
Proposed approach: NAR = 0.0725, which is better.


## 2. Proposed Method

1. Preprocessing:

- Resize images to 224×224 pixels.
- Two resizing methods are tested: scaling and padding.

2. Feature Extraction:

- Two pretrained CNN models (ResNet-50 and VGG-16) are used to extract features.

3. Feature Reduction:

- Principal Component Analysis (PCA) is applied to reduce feature dimensions and improve efficiency.
4. Similarity Measurement:
- Euclidean distance is used to calculate the similarity between query and registered trademarks.
5. Evaluation Metrics:
- Average rank, Normalized Average Rank (NAR), and Mean Average Precision (mAP).


