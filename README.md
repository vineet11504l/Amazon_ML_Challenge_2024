# Amazon ML Challenge 2024

This repository contains our solution to the **Amazon ML Challenge 2024**, where the objective was to extract product dimensions from images and maximize the F1 score. Competing against over 10,000 teams, we secured the **31st position** with an impressive F1 score of **0.65**.

## Objective
The primary goal of this challenge was to extract accurate product dimensions (height, width) from product images by analyzing textual and visual features. 

---

## Approach
Our solution combined state-of-the-art optical character recognition (OCR) techniques and image processing algorithms to extract, clean, and standardize product dimensions from images. Below is an overview of our methodology:

### 1. Text Extraction using PaddleOCR
We applied **PaddleOCR** to extract text from product images efficiently:
- Extracted text included numerical values and their associated units.
- Utilized **regular expressions (regex)** to clean the extracted text and isolate meaningful numerical values along with their corresponding units.

### 2. Estimating Product Dimensions
- Applied **Hough Line Transformation** to detect lines and orientations within the image.
- Used bounding box orientations to determine and estimate the **height** and **width** of the product.

### 3. Standardization and Post-Processing
- Implemented a robust **unit standardization mapping** to ensure uniformity across the extracted dimensions.
- This step was critical for achieving a high F1 score by normalizing the data dimensions effectively.

---

## Files in this Repository

1. **`extracting_text_from_images.ipynb`**
   - This notebook demonstrates the process of text extraction using PaddleOCR.
   - Includes regex-based cleaning and isolation of numerical values with their respective units.

2. **`getting_product_dimensions.ipynb`**
   - This notebook contains the logic for estimating product dimensions.
   - Covers the implementation of Hough Line Transformation, bounding box analysis, and unit standardization.

---

## Results
- **F1 Score:** 0.65
- **Rank:** 31st out of 10,000+ teams



## Acknowledgments
We extend our gratitude to Amazon for hosting this exciting challenge and providing an engaging platform to solve real-world problems using machine learning and computer vision.

---

## Contact
For any queries or discussions, feel free to reach out via:
- Email: [aadishjin54321@gmail.com.com](mailto:aadishjain)
- GitHub Issues: [Open an issue](https://github.com/ajax1310/amazon-ml-challenge-2024/issues)

---

Thank you for visiting our repository! We hope you find our solution insightful.
