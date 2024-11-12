***Question 1***

  The original RGB image was converted to grayscale. After converting the image to grayscale, we applied a Gaussian blur to smooth the image. This reduces noise and small details, making it easier to detect obvious edges. The smoothed image appears sligtly blurred compared to the grayscale version but not in a drastic way.

***Question 2***

  To detect edges, we applied Sobel filters along both the x and y directions to compute the gradients. The Sobel filter highlights regions where there are sudden changes in intensity, which are typically the edges in the image. The gradient magnitude was then calculated from the x and y gradients to create the final edge-detected image. The edge-detected image shows the outlines of the lion and prominent features like the mane and face being recognizable, as well as some parts of the foreground and ground. The background is mostly dark meaning there is little to no intensity change.