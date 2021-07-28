
### Feature extraction

<details open>
  <summary> Sobel filter </summary>
 
</details>

<details open>
  <summary> Sobel filter </summary>
    
 * Edge detection algorithm.

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
  <summary> SIFT (Scale Invariant Feature Transform) </summary>
 
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

* Main components of visual tracking
  * Target initialization (Bounding box)
  * Appearance modeling (Feature extraction)
  * Motion model 
    * Motion estimation
    * Motion update

* Types of visual tracking
  * Meanshift and Cam shift 
  * Lukas Kanade 
  * Convolution based (Go-turn)

* Types of Optical flow:
  * Sparse optical flow
  * Dense optical flow   

* Optical flow working
  *  2D vector field where each vector is a displacement vector showing the movement of points from first frame to second.


#### Reference
1. https://cv-tricks.com/object-tracking/quick-guide-mdnet-goturn-rolo/




