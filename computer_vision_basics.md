
### Feature extraction

<details open>
  <summary> The Sobel and Laplacian Edge Detectors </summary> 
 
 [(src)](https://aishack.in/tutorials/sobel-laplacian-edge-detectors/)
 *  Sobel edge detector    
    * Gradient based edge detection (1st derivative).
    * If color change is very steep it is an edge.
    * 2 kernels (Gx) and (Gy) are used. 
 * Laplacian edge detector    
   * 2nd Derivative based edge detection.
   * Extremely sensitive to noise due to 2nd order derivative.
   * Single kernel for both directions and directly get 2nd order derivative. 
   * Computationally faster to calculate

</details>

<details open>
  <summary> Gaussian filter </summary>
 
 * Discrete approximation using kernel matrix and convolve it. 
 * Reduce image noise and blur/smoothen edges in image.
 * Low-pass filter
</details>


<details open>
  <summary> Canny edge detection </summary>
 
  * Color transform to Greyscale
  * Gx and Gy intensity grad
 
</details>



<details open>
  <summary> Different Feature extraction algorithms </summary>
 
  * Edge detection
    * Sobel filter
    * Prewitt filter  
    * Canny edge detector
  * Corner detection
    * Harris corner
    * Shi–Tomasi
 
 </details>

<details open>
  <summary> Gaussian pyramid and Laplacian pyramid </summary>

  * Used for multi scale representation and can be used for extracting multi-scale features.
  * Gaussian pyramid:
    * Uses Gaussian blur between subsequent downsampled image
 
</details>
 
<details open>
  <summary> SIFT (Scale Invariant Feature Transform)  </summary>
 
  * General steps for SIFT [(src)](https://aishack.in/tutorials/sift-scale-invariant-feature-transform-introduction/):
    * Scale space generation (4 octaves and 5 blurs)
    * LoG approximations (Difference of Gaussians)
    * Locate key points 
        * Locate maxima/minima in DoG images (Compare 26 neighbors)
        * Find subpixel maxima/minima (Interpolation)
    * Remove bad keypoints
      * Removing low contrast features (General intensity comparison)
      * Remove edges and flat regions (corners are good features)
    * Keypoint orientations
      * Calculate magnitude and orientation
      * Histogram (360 degrees of orientation are broken into 36 bins)
    * Create feature vectors from this (128D)
      * 16 x 16 grid around (4x4 grids)
      * Use orientations and magnitudes to create histograms
  
</details>

<details open>
  <summary> Hough transform </summary>

  * Method to find shape in the image.
  * Uses polar coordinates. 
  * Accumulator : 
  * General steps :
    1. Extract edges in image
    2. Choose desired transformations
    3. Iterate through image and populate the accumulator 
    4. Search local maximum values in accumulator space 
 
</details>


--------------
### Object detection

--------------
### Segmentation

--------------
### Tracking [1]

<details open>
  <summary> Main components of visual tracking </summary>

  * Target initialization (Bounding box)
  * Appearance modeling (Feature extraction)
  * Motion model 
    * Motion estimation
    * Motion update
</details>

<details open>
  <summary> Types of visual tracking </summary>

  * Meanshift and Cam shift 
  * Lukas Kanade 
  * Convolution based (Go-turn)
</details>

<details open>
  <summary> Types of Optical flow </summary>

  * Sparse optical flow
  * Dense optical flow   

</details>

<details open>
  <summary> Optical flow working </summary>
 
  *  2D vector field where each vector is a displacement vector showing the movement of points from first frame to second.

</details>

#### Reference
1. https://cv-tricks.com/object-tracking/quick-guide-mdnet-goturn-rolo/




