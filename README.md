# Computer Vision Fundamentals

A collection of practical computer vision implementations exploring fundamental techniques in image processing, feature extraction, classification, video analysis, and motion detection.

The project consists of five Jupyter notebooks covering progressively different areas of classical computer vision.

## Projects

### 1. Image Transformations
Implements image rotation and horizontal skewing using affine transformations. Experiments compare forward and inverse mapping, interpolation methods, and the effect of changing the order of transformations.

### 2. Convolution and Image Filtering
Implements 2D convolution and explores averaging, Gaussian-like smoothing, and Laplacian edge detection. Different kernel sizes, shapes, and combinations are compared to investigate their effects on image detail and structure.

### 3. Video Segmentation
Uses RGB colour histograms and histogram intersection to measure similarity between video frames. The approach is applied to consecutive frames to explore simple scene-change detection and temporal variation.

### 4. Texture Classification
Extracts Local Binary Pattern (LBP) features from image regions and combines them into global image descriptors. Histogram intersection and 1-nearest-neighbour classification are then used to distinguish between face and non-face images.

### 5. Motion-Based Object Counting
Detects and counts moving vehicles in video using frame differencing, thresholding, temporal background estimation, morphological processing, and connected-component analysis.

## Technologies

- Python
- OpenCV
- NumPy
- Matplotlib
- SciPy
- scikit-image
- scikit-learn
- Jupyter Notebook

## Repository Structure

```text
computer-vision-fundamentals/
├── 01_image_transformations.ipynb
├── 02_convolution_filtering.ipynb
├── 03_video_segmentation.ipynb
├── 04_texture_classification.ipynb
├── 05_object_counting.ipynb
├── requirements.txt
└── README.md
