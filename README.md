# Roof Edge Detection & Contour Extraction using OpenCV

This project implements a complete computer vision pipeline for extracting clean roof contours from aerial images.  
It converts raw input photos into high-contrast black-line drawings and exports contour coordinates for further analysis (CAD, ML, GIS, etc.).

---

## ✨ Features

- Load aerial roof images (manual path or Colab upload)
- Preprocessing:
  - Grayscale conversion  
  - Gaussian blur  
  - Optional heavy noise reduction  
  - Morphological smoothing  
- Edge detection using Canny  
- Automatic extraction of the **largest roof contour**  
- 🖼️ Output generation:
  - Black contour on white background
  - Contour overlay on original image
  - Raw edges visualization
- 📁 Automatic output folder creation (`/drawing`, `/output`)
- CSV export of contour coordinates
- Fully modular Python code (easy to extend)

---

## 🖥️ Technologies Used

- **Python 3**
- **OpenCV**
- **NumPy**
- **Matplotlib**

---

# How to run

You can copy this repository into Google Colab and run the project in a few steps:

1. Upload the entire repo (or clone it) into your Colab workspace.
2. Make sure the `Sample/` folder with images is present.
3. Open the `.ipynb` notebook file.
4. Run each cell made for colab from top to bottom.

No additional configuration is required.  
The notebook installs the correct versions of OpenCV and NumPy automatically.

Otherwise, copy this repository locally:

1. Clone or download the repo
2. Install the required Python packages
   - gensim 4.3.3 requires numpy<2.0,>=1.18.5
   - numba 0.60.0 requires numpy<2.1,>=1.22
   - scipy 1.13.1 requires numpy<2.3,>=1.22.4

   !pip install "opencv-python<4.9.0" --force-reinstall
   !pip install numpy==1.26.4 --force-reinstall
   
3. Ensure the `Sample/` folder is present and contains your input images.
4. Open `.ipynb` in jupiter notebook (or other IDEE of your choice)
5. Run each cell made for local use from top to bottom.

---

