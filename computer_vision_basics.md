
### Feature extraction

* Sobel filter
  * Edge detection algorithm.
  * 

* Gaussian filter
  * Discrete approximation using kernel matrix and convolve it. 
  * Reduce image noise and blur/smoothen edges in image.
  * Low-pass filter

* Different Feature extraction algorithms:
  * Edge detection
    * Sobel filter
    * Prewitt filter  
  * Corner detection
    * Harris corner
    * Shi–Tomasi

* Gaussian pyramid and Laplacian pyramid
  * Used for multi scale representation and can be used for extracting multi-scale features.
  * Gaussian pyramid:
    * Uses Gaussian blur between subsequent downsampled image
    *  

* SIFT (Scale invariant feature transform)
  *  

* Hough transform
  * Method to find shape in the image.
  * Uses polar coordinates. 
  * Accumulator : 
  * General steps :
    1. Extract edges in image
    2. Choose desired transformations
    3. Iterate through image and populate the accumulator 
    4. Search local maximum values in accumulator space 

*  

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




