### Transformations
<details open>
  <summary> Homogeneous transformation</summary>
  
</details>

<details open>
  <summary> Types of Transformations </summary>
 
  1. Euclidean Transformations (Translations and Rotations on the xy-Plane)    
  2. Affine transformation (Scaling and shear)    
  3. Projective transformation (also called perspective transform or homography or collineation)    
</details>

<details open>
  <summary> Types of angle representations </summary>
  
  * Euler angles 
  * Axis/angle
  * quaternions
</details>

<details open>
  <summary> Isotropic vs Non-Isotropic scaling </summary>
  
* Isotropic scaling
    * Same scaling factor along width and height. 
    * ie. Maintains Aspect ratio
* Non-Isotropic scaling 
    * Uses different scaling factor along width and height.
    * ie. Dosn't maintains aspect ratio
</details>

<details open>
  <summary> Ideal points </summary>
  
  * Points where parallel lines meet at infinity in homogeneous coordinate systems.
  * (x,y,0) --> in homogeneous coordinates
</details>

<details open>
  <summary> Homogeneous coordinate into Eucledian coordinate system </summary>
  
   * Converting from a homogeneous coordinates to a conventional one is unique; but, converting a conventional coordinates to a homogeneous one is not. 
  * (x,y) in the xy-plane is (xw, yw, w) for any non-zero w. (Non-unique)
</details>

### Calibration

<details open>
  <summary> Calibration </summary>
  
  * Calibration is the process of estimating the camera matrix ie. extrinsic and intrensic paprameters (K) of a camera.
</details>

<details open>
  <summary> Camera Matrix </summary>
  
  * Camera matrix transforms 3D point in the world to 2D point on the image plane.  
  * It can be decomposed into 2 components:
    * Intrinsic parameters
    * Extinsic parameters
  * 3D points ---(Extrinsic matrix)---> Camera coordinates ---(Intrinsic parameters)---> Image plane 
</details>

<details open>
  <summary> What are the intrinsic properties of a camera? </summary>
  
  [(src)](https://ksimek.github.io/2012/08/22/extrinsic/)
  * Image center (cx, cy)
  * Focal length (fx, fy)
  * Lens distorsion parameters.
</details>

<details open>
  <summary> What are the extrinsic properties of a camera? </summary>
  
  [(src)](https://ksimek.github.io/2012/08/22/extrinsic/)
  * Extrinsic [R|t] transform points in world coordinates into camera coordinates.
  * Components of extrinsic matrix
    * R --> Rotation matrix 
    * t --> Translation vector
</details>

<details open>
  <summary> Types of distorsion? </summary>
  
  * Radial distorsion
  * Tangential distorsion
</details>


----------
#### Extra References
<details open>
   <summary> Links </summary>
  1. https://pages.mtu.edu/~shene/COURSES/cs3621/NOTES/

</details>
