# GPU-Accelerated Batch Image Processing Using CUDA

## Project Overview

GPU-Accelerated Batch Image Processing is a parallel computing project that uses NVIDIA CUDA to process multiple high-resolution images efficiently. The project implements image-processing operations such as grayscale conversion, Gaussian blur, and Sobel edge detection using GPU parallel processing.

The system processes a batch of 10 images (1080 × 1980 pixels) and compares CPU-based processing with GPU-based processing to analyse execution time, computational efficiency, and performance improvement.

By utilizing CUDA threads to execute image-processing operations in parallel, the project demonstrates how GPU computing can accelerate computationally intensive tasks compared to traditional CPU processing.

## Objectives

- To implement image-processing operations using CUDA.
- To understand GPU parallel processing and thread execution.
- To process multiple high-resolution images in batches.
- To compare CPU and GPU execution time.
- To analyse GPU performance using speedup calculations.

## Image Processing Operations

### 1. Grayscale Conversion
Converts colour images into grayscale images by transforming pixel colour values into intensity values.

### 2. Gaussian Blur
Applies Gaussian filtering to reduce noise and smooth the image by averaging neighbouring pixel values using a Gaussian kernel.

### 3. Sobel Edge Detection
Detects edges in images by calculating intensity gradients in horizontal and vertical directions to identify boundaries and structural details.

## Technologies Used

- C++
- NVIDIA CUDA
- OpenCV
- CMake
- Google Colab
- NVIDIA GPU (Tesla T4)

## Dataset

- Number of images: 10
- Image resolution: 1080 × 1980 pixels
- Image format: JPG

## Project Structure

```text
GPU-Batch-Image-Processing/
│
├── README.md
├── CMakeLists.txt
│
├── src/
│   ├── batch_processor.cpp
│   ├── image_processing.cu
│   └── image_processing.h
│
├── dataset/
│   └── sample_images/
│
├── output/
│   ├── grayscale/
│   ├── blur/
│   └── edges/
│
├── results/
│   └── performance.csv
│
└── screenshots/
```

## Workflow

1. Load input images from the dataset directory.
2. Perform image processing using CPU implementation.
3. Perform image processing using CUDA GPU implementation.
4. Generate grayscale, Gaussian blur, and edge-detection outputs.
5. Measure CPU and GPU execution times.
6. Calculate performance speedup.
7. Store processed images and performance results.

## Performance Analysis

The project compares CPU and GPU execution time for batch image processing.

| Metric | Description |
|---|---|
| CPU Execution Time | Time taken by CPU to process the batch |
| GPU Execution Time | Time taken by GPU to process the batch |
| Speedup | CPU execution time divided by GPU execution time |

Speedup Formula:

**Speedup = CPU Execution Time / GPU Execution Time**

Performance results are stored in `results/performance.csv`.

## Expected Outcomes

- Faster image-processing execution using GPU parallelism.
- Understanding of CUDA kernel execution.
- Comparison of CPU and GPU computational performance.
- Demonstration of parallel computing for image-processing applications.

## Conclusion

This project demonstrates the application of NVIDIA CUDA in accelerating batch image-processing tasks using GPU parallel computing. By implementing grayscale conversion, Gaussian blur, and Sobel edge detection, the project evaluates the performance differences between CPU and GPU implementations and highlights the benefits of parallel processing for computationally intensive workloads.

---

**Developed as a Parallel Computing / GPU Computing project.**
