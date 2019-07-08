# CT-Tutorial
Tutorial code for CT reconstruction with high dynamic range images.  See the 
[Landing page](https://pages.github.rcac.purdue.edu/GregeryBuzzardGroup/CT-Tutorial/)
for more details.  

### Conversion of a CT image to a noisy sinogram and reconstruction with noise and without noise.  

This notebook is a tutorial on reconstruction of high-dynamic range CT images with proper physical scaling and a realistic noise model. 

**Outline of processing:**

1. Read image: in Hounsfield units (air=0, water=1000)
- Scale so that air=0, water=1
- Mask for circular ROI
- Take the raw sinogram using a specified number of views
- Scale to account for pixel pitch and x-ray density
- Add noise to the sinogram using the correct variance
- Reconstruct from the original and noisy sinogram
- Display the reconstructions and sinograms

See CT_Tutorial.ipynb for more details.  The file make_data.ipynb includes code to create high dynamic range images.  
