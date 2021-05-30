### Imaging Science

* Ideal imaging sensor: 
  * No noise
  * Infinite pixels
  * Infinite fps
  * Infinite Dynamic range 
  * Infinite SNR

* Signal/Noise ratio
  * Electronics always have an inherent noise
  * Ratio of the measured signal to the underlying noise (SNR)
  * High SNR -> Good, Low SNR -> Noisy image

* ISO and gain 
  * Electornic amplification of the system
  * Causes increase in signal and noise   

* General sensor characterstics
  * Noise floor (read noise)
  * Dynamic range
  * Saturation level (Full well capacity)
  * Responsivity     

* Types of Noise
    * Fixed pattern noise:
      * Predictable distribution due to structure
      * Long exposure, Low ISO
      * Dark signal non-uniformity, Pixel response non-uniformity 
      * Fixed for each sensor
    * Random noise: 
      * Unpredictable distribution (Not constant for each frame)
      * Short exposure, High ISO 
      * Averaging used to reduce
    * Banding noise: 
      *  Sensor readout noise
      *  Can be removed for each sensor

* Methods to reduce noise:
  * Increase lightning (More SNR)
  * Increase shutter speed/ Widen aperture/ Increase exposure
  * Low temperature
  * Filters: Gaussian, Median, Mean

* Bayer array
  * Grid filter array of RGB pattern
  * Twice as many green as red or blue sensors 

* Non bayer filters
  * The Fujifilm X-Trans sensor 
  * Super CCD

* Demosaicing
  * In bayer filter cameras 
  * Reconstructing images from bayer RAW
  * Small scale details lead to artifacts

* CMOS vs CCD
  * Charged-Coupled Device   
    * Global shutter
    * Vertical smear
    * Readout in corners
  * Complementary Metal–Oxide–Semiconductor
    * Rolling shutter
    * Problems in low lights and flikering lights
    * Better battery
    * Readout @ each pixel

## References
1. https://www.eecs.tu-berlin.de/fileadmin/fg144/Courses/10WS/pdci/talks/noise_sensors.pdf
2. https://www.cambridgeincolour.com/learn-photography-concepts.htm
3. https://skyandtelescope.org/astronomy-blogs/imaging-foundations-richard-wright/dark-frames-and-bias-frames-demystified/
