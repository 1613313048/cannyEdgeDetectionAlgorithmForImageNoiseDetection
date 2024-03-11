# cannyEdgeDetectionAlgorithmForImageNoiseDetection
The Canny edge detector is an edge detection operator that uses a multi-stage algorithm to detect a wide range of edges in images. It was developed by John F. Canny in 1986. Canny also produced a computational theory of edge detection explaining why the technique works.

The Canny edge detection algorithm is composed of 5 steps:
1)Gaussian Blur.
2)Sobel Operation.
3)Non-maximum suppression.
4)Double threshold.
5)Edge Tracking by Hysteresis.

1.Gaussian Blur: Since edge detection is susceptible to noise in the image first step is to remove the noise in the image with a Gaussian Filter.

2.Sobel Operation: Smoothened image is then filtered with a sobel kernel is both X and Y direction to get derivatives Gx and Gy. From this we get gradient intensity matrix and gradient angles.

3.Non Maximum Suppression: The final image should have thin edges. Thus,we must perform non-maximum suppression to thin out the edges.
Algorithm: the algo goes through all points on the image and finds the pixels with the maximum value of gradient in the edge directions.

4. Double thresholding: Remaining edge pixels after non-maximum suppression provide a more realistic representation of real edges in an image. However, noise and colour change continue to generate some edge pixels. In order to explain these erroneous answers,Edge pixels with a low gradient value must be filtered removed, whereas edge pixels with a high gradient value must be preserved.

5.Edge tracking by Hysteresis: As far as we know, the strong edge pixels should be included in the final edge image because they are taken from the image's genuine edges. However, there will be some disagreement over the weak edge pixels, which can be retrieved from either the genuine edge or the noise/color variations. The weak edges created by the latter explanations should be eliminated to achieve an accurate outcome.




   









      
