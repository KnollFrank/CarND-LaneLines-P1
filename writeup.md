# **Finding Lane Lines on the Road**

## Writeup

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report


[//]: # (Image References)

[image1]: ./examples/grayscale.jpg "Grayscale"

---

### Reflection

### Pipeline

TODO: Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

The pipeline performs the following steps:
1. Given an image:<br> ![original](test_images_output_improved/solidYellowLeft_original.png)
2. Convert the image to grayscale:<br> ![grayscale](test_images_output_improved/solidYellowLeft_grayscale.png)
3. Blur the image using a Gaussian filter:<br> ![gaussian_blur](test_images_output_improved/solidYellowLeft_gaussian_blur.png)
4. Find edges in the image using the Canny algorithm:<br> ![canny](test_images_output_improved/solidYellowLeft_canny.png)
5. Keep a polygonal region of the image probably containing lane lines:<br> ![region_of_interest](test_images_output_improved/solidYellowLeft_region_of_interest.png)
6. Find lane lines in the image using the (probabilistic) Hough transform:
   - original draw_lines():<br> ![hough_lines](test_images_output/solidYellowLeft_hough_lines.png)
   - modified draw_lines():<br>
 ![hough_lines](test_images_output_improved/solidYellowLeft_hough_lines.png)
 7. Draw the lane lines found in the previous step onto the original image:
    - original draw_lines():<br> ![weighted_img](test_images_output/solidYellowLeft_weighted_img.png)<br>
    - modified draw_lines():<br> ![weighted_img](test_images_output_improved/solidYellowLeft_weighted_img.png)

In order to draw a single line on the left and right lanes, I modified the draw_lines() function by ...

If you'd like to include images to show how the pipeline works, here is how to include an image:

![alt text][image1]


### 2. Identify potential shortcomings with your current pipeline


One potential shortcoming would be what would happen when ...

Another shortcoming could be ...


### 3. Suggest possible improvements to your pipeline

A possible improvement would be to ...

Another potential improvement could be to ...
