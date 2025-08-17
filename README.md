# Image Compression Using PCA

## Overview

This project demonstrates image compression using Principal Component Analysis (PCA) in Python. By applying PCA to each color channel (RGB) of an image, the algorithm significantly reduces file size while retaining a high percentage of the original image's variance and visual quality.

## Features

- Loads and analyzes an image (JPG/JPEG/PNG)
- Performs PCA on each image channel
- Saves compressed image with reduced dimensions
- Displays explained variance and compression ratio
- Visualizes variance per principal component


### 2. Main Functions

- **img_data(imgPath, disp=True)**  
  Loads image and returns dimensions and file size.

- **pca_compose(imgPath)**  
  Conducts PCA decomposition on each color channel.

- **explained_var_n(pca_channel, n_components)**  
  Calculates total explained variance by the top `n_components`.

- **variance_added_pc(pca_channel)**  
  Computes incremental variance added by each principal component.

- **plot_variance_pc(pca_channel)**  
  Plots variance explained by principal components.

- **pca_transform(pca_channel, n_components)**  
  Compresses the image with the specified number of components and reconstructs it.


## Results

- **Preserves >99% variance** of the original image with considerably fewer components.
- **Compression ratio:** Over 80% reduction in file size (as shown in the code sample).
- **Retains visual quality**: The compressed image remains visually similar to the original.

## Dependencies

- numpy
- pillow
- matplotlib
- scikit-learn

## Applications

- Efficient image storage and transmission
- Demonstration of dimensionality reduction on real-world images
- Educational tool for PCA in image processing

## License

This project is MIT licensed.

---

*Author: Saniya Chhabra  




