# Computer Vision Fundamentals

### Classical computer vision techniques for image transformation, filtering, texture analysis, video segmentation and motion detection

A collection of practical computer vision projects implemented in Python and OpenCV.

The repository explores core computer vision techniques from first principles, including geometric transformations, convolution, texture descriptors, histogram-based video analysis and motion-based object detection.

## Project overview

The project is organised into five notebooks:

| Notebook | Topic | Main techniques |
| --- | --- | --- |
| `01_image_transformations.ipynb` | Image transformations | rotation, skewing, affine transforms, interpolation |
| `02_convolution_filtering.ipynb` | Convolution and filtering | smoothing, averaging filters, Laplacian edge detection |
| `03_video_segmentation.ipynb` | Video segmentation | RGB histograms, histogram intersection, frame comparison |
| `04_texture_classification.ipynb` | Texture classification | Local Binary Patterns, histogram descriptors, nearest-neighbour classification |
| `05_object_counting.ipynb` | Motion-based object counting | frame differencing, background estimation, morphology, connected components |

## What I implemented

- affine image rotation and skew transformations;
- full-canvas rotation to avoid clipping transformed images;
- comparison of interpolation methods including nearest-neighbour, linear, cubic and Lanczos;
- custom image-filtering and convolution experiments;
- smoothing and Laplacian edge-detection filters;
- RGB histogram extraction from video frames;
- histogram-intersection similarity for temporal frame comparison;
- Local Binary Pattern feature extraction;
- regional histogram descriptors for texture representation;
- nearest-neighbour texture classification;
- reference-frame and temporal frame differencing;
- threshold-based motion segmentation;
- temporal background estimation;
- morphological mask processing;
- connected-component analysis for moving-object detection and counting.

## Image transformations

The first notebook explores geometric image manipulation using affine transformations.

Rotation and skew operations are applied while accounting for changes in output dimensions so transformed images are not unnecessarily cropped.

Additional experiments compare different interpolation methods and demonstrate how transformation order affects the final result.

## Convolution and image filtering

The second notebook explores spatial filtering through two-dimensional convolution.

Different kernels are used to investigate:

- image smoothing;
- averaging filters;
- Gaussian-like filtering;
- edge detection using Laplacian operators;
- the effect of kernel size and structure on image detail.

## Video segmentation

The third notebook analyses changes between video frames using colour information.

RGB histograms are extracted from individual frames and compared using histogram intersection.

Changes in histogram similarity provide a simple classical method for identifying temporal variation and potential scene transitions.

## Texture classification

The fourth notebook represents image texture using Local Binary Patterns.

The pipeline:

1. divides images into local regions;
2. calculates LBP codes for neighbouring pixels;
3. creates local histograms;
4. concatenates them into image-level descriptors;
5. compares descriptors using histogram similarity;
6. applies nearest-neighbour classification.

This demonstrates how engineered visual features can be used for classification without a deep neural network.

## Motion-based object counting

The final notebook detects movement in video using frame-level differences.

The processing pipeline combines:

1. frame differencing;
2. grayscale difference maps;
3. thresholding;
4. temporal background estimation;
5. morphological processing;
6. connected-component analysis.

These steps progressively convert raw pixel changes into regions corresponding to moving objects.

## Repository structure

```text
computer-vision-fundamentals/
├── 01_image_transformations.ipynb
├── 02_convolution_filtering.ipynb
├── 03_video_segmentation.ipynb
├── 04_texture_classification.ipynb
├── 05_object_counting.ipynb
├── requirements.txt
├── .gitignore
└── README.md
