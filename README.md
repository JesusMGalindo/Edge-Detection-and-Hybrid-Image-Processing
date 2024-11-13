##  Vicente Ramos & Jesus Galindo

### Part A

**Question 1**

  The original RGB image was converted to grayscale. After converting the image to grayscale, we applied a Gaussian blur to smooth the image. This reduces noise and small details, making it easier to detect obvious edges. The smoothed image appears slightly blurred compared to the grayscale version but not in a drastic way.

**Question 2**

  To detect edges, we applied Sobel filters along both the x and y directions to compute the gradients. The Sobel filter highlights regions where there are sudden changes in intensity, which are typically the edges in the image. The gradient magnitude was then calculated from the x and y gradients to create the final edge-detected image. The edge-detected image shows the outlines of the lion and prominent features like the mane and face being recognizable, as well as some parts of the foreground and ground. The background is mostly dark meaning there is little to no intensity change.

  ### Part B

  **Low pass**
  For the first two images A and B, we applied a gaussian blur using 23x23 for the kernel size and 5 for the sigma. This will make the image smooth, while also maintain the low frequency components. Some of the low frequency components highlighted in the image are the colors for the lion and background. While the high frequency components are textures and the edges which are more difficult to see.

  **High pass**
  Our approach was to subtract the low pass filtered version of our original lion image. By subtraction the low pass filter in the last problem we are isolating the high frequency components. This leads to an output that highlights the edges and finer details of the image.

  **Hybrid**

  For the hybrid approach we combined both low pass and high pass filters by applying weights to the images. This created an image where we get the best of both filters. By doing applying 0.5 weights to both images we get the high frequency detailing emphasizing the close-up details while also mainlining the low frequency details which makes it easier to see what the image is from further away. 

  For all 3 approaches we tested with different kernel sizes and paraments. This helped us solidify the significance differences between each approach. The increasing or decreasing paraments we can exaggerate the implementation for low, high and hybrid approach.
