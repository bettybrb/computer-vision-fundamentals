# Computer Vision Fundamentals

### Classical computer vision techniques for image transformation, filtering, texture analysis, video segmentation and motion detection

A collection of five practical computer vision projects implemented in Python and OpenCV.

The repository explores core computer vision techniques from first principles, including geometric transformations, convolution, texture descriptors, histogram-based video analysis and motion-based object detection.

## Project overview

| Notebook | Topic | Main techniques |
| --- | --- | --- |
| `01_image_transformations.ipynb` | Image transformations | rotation, skewing, affine transforms, interpolation |
| `02_convolution_filtering.ipynb` | Convolution and filtering | smoothing, averaging filters, Laplacian edge detection |
| `03_video_segmentation.ipynb` | Video segmentation | RGB histograms, histogram intersection, frame comparison |
| `04_texture_classification.ipynb` | Texture classification | Local Binary Patterns, histogram descriptors, nearest-neighbour classification |
| `05_object_counting.ipynb` | Motion-based object counting | frame differencing, background estimation, morphology, connected components |

## What I implemented

- affine image rotation and skew transformations
- full-canvas rotation to avoid clipping transformed images
- comparison of nearest-neighbour, linear, cubic and Lanczos interpolation
- image convolution and filtering experiments
- smoothing and Laplacian edge-detection filters
- RGB histogram extraction from video frames
- histogram-intersection similarity for temporal comparison
- Local Binary Pattern feature extraction
- regional histogram descriptors for texture representation
- nearest-neighbour texture classification
- frame differencing and background estimation
- threshold-based motion segmentation
- morphological mask processing
- connected-component analysis for moving-object detection and counting

## Image transformations

The first notebook explores geometric image manipulation using affine transformations.

Rotation and skew operations are applied while accounting for changes in output dimensions so transformed images are not unnecessarily cropped. Additional experiments compare interpolation methods and demonstrate how transformation order affects the final result.

## Convolution and image filtering

The second notebook explores spatial filtering through two-dimensional convolution.

The experiments investigate smoothing, averaging filters, Gaussian-like filtering and Laplacian edge detection, showing how different kernels affect image detail and structure.

## Video segmentation

The third notebook analyses visual changes between video frames.

RGB histograms are extracted from individual frames and compared using histogram intersection. Changes in similarity provide a simple classical method for analysing temporal variation and potential scene transitions.

## Texture classification

The fourth notebook represents image texture using Local Binary Patterns.

Images are divided into local regions, LBP codes are calculated, local histograms are created and combined into image-level descriptors, and nearest-neighbour classification is used to compare textures.

## Motion-based object counting

The final notebook detects movement in video using differences between frames.

Frame differencing, thresholding, temporal background estimation, morphological processing and connected-component analysis progressively convert pixel changes into regions corresponding to moving objects.

## Repository structure

    computer-vision-fundamentals/
    ├── 01_image_transformations.ipynb
    ├── 02_convolution_filtering.ipynb
    ├── 03_video_segmentation.ipynb
    ├── 04_texture_classification.ipynb
    ├── 05_object_counting.ipynb
    ├── requirements.txt
    ├── .gitignore
    └── README.md

## Tech

**Python · OpenCV · NumPy · Matplotlib · SciPy · scikit-image · scikit-learn · Jupyter · affine transformations · image convolution · spatial filtering · Local Binary Patterns · histogram analysis · video processing · motion detection · morphological processing · connected-component analysis**
