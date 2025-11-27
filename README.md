# GEL_ELECTROPHOROSIS
Automated DNA gel electrophoresis band detection using C++, OpenCV, and OpenMP. The system performs noise reduction, thresholding, edge detection, and contour-based band identification. Parallel processing accelerates execution, producing fast and accurate annotated gel images.
Here is your **exact README**, perfectly formatted and ready to **copy–paste directly into GitHub**:

---

#  Parallel DNA Gel Electrophoresis Band Detection Using OpenMP & OpenCV

This project implements a high-performance DNA gel electrophoresis band detection system using C++, OpenCV, and OpenMP, with optional visualization through Python. The system automates the detection of DNA bands from electrophoresis gel images by applying an optimized image-processing pipeline and accelerating computation using parallel processing.

---

##  Key Features

### 1. Automated Gel Image Processing

The project uses a multi-stage pipeline consisting of:

* **Gaussian Blur** for noise reduction
* **Adaptive Thresholding** for segmentation under uneven lighting
* **Morphological Operations** for noise cleaning
* **Sobel Edge Detection** for enhanced band boundary detection

###  2. Parallel Processing with OpenMP

Computationally expensive stages are parallelized using OpenMP, delivering:

* Faster execution time
* Improved performance on multi-core CPUs
* Scalability for batch gel image analysis

### 🔹 3. Band Detection using Contours

The system identifies bands using:

* Binary thresholding
* Contour extraction
* Bounding-box generation
* Automated annotation of detected band regions

### 🔹 4. Python Visualization (Optional)

Python is used to:

* Display intermediate stages
* Show the final annotated image
* Provide a user-friendly interface

---

##  Included in This Repository

* **gel_processing.cpp**
  → Main C++ file with OpenCV + OpenMP pipeline

* **Annotated_Bands.jpg**
  → Output with detected DNA bands highlighted

### Intermediate image outputs:

* Original_Gel_Image.jpg

* Blurred_Image.jpg

* Thresholded_Image.jpg

* Sobel_Edges.jpg

* **(Optional) .ipynb Google Colab Notebook**
  → Full run: install → compile → run → visualize

---

## 🚀 How It Works

1. Load Gel Image (supports GEL.jpg / gel.jpg / jpeg / JPG…)
2. Apply Gaussian Blur to smooth noise
3. Adaptive Thresholding (binary inversion for contour detection)
4. Morphological Cleaning (remove speckles)
5. Sobel Edge Map computation
6. Contour Detection to locate band regions
7. Draw Bounding Boxes around detected bands
8. Save Final Annotated Output

---

## Technologies Used

* C++
* OpenCV 4
* OpenMP (parallel processing)
* Python (optional)
* Google Colab (development & execution environment)

---

##  Purpose of This Project

This project was developed as part of the **Computer Architecture & Organization (BITE301L)** laboratory requirement.
It demonstrates:

* Practical application of parallel computing
* Use of image processing techniques in bioinformatics
* Real-world performance comparison between CPU and GPU workflows
* Integration of C++ and Python for hybrid systems

---

##  Results (Sample)

The optimized pipeline delivers:

* ✓ Automatic detection of DNA lanes and band regions
* ✓ Reduction in manual analysis time
* ✓ Improved accuracy under non-uniform lighting
* ✓ Performance boost with OpenMP multithreading

---

## Future Enhancements

This project can be extended by adding:

* Machine learning–based band classification
* Quantification of DNA band intensity
* Lane segmentation & labeling
* Full gel profiling for research use
