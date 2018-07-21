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

My pipeline consisted of 5 steps.
1. Given an image:<br/>
![original](test_images_output_improved/solidYellowLeft_original.png)
2. I converted the image to grayscale:<br/>
![grayscale](test_images_output_improved/solidYellowLeft_grayscale.png)
3. bla<br/>
![gaussian_blur](test_images_output_improved/solidYellowLeft_gaussian_blur.png)
4. blub<br/>
![canny](test_images_output_improved/solidYellowLeft_canny.png)
5. sdf<br/>
![region_of_interest](test_images_output_improved/solidYellowLeft_region_of_interest.png)
6.sdf<br/>
![hough_lines](test_images_output_improved/solidYellowLeft_hough_lines.png) oder ![hough_lines](test_images_output/solidYellowLeft_hough_lines.png)
7. sdf<br/>
![weighted_img](test_images_output_improved/solidYellowLeft_weighted_img.png) oder ![weighted_img](test_images_output/solidYellowLeft_weighted_img.png)

Description  | not improved  | pipeline  | improved
--|---|---|--
Given an image:  |   | ![original](test_images_output_improved/solidYellowLeft_original.png)  |  
I converted the image to grayscale:  |   | ![grayscale](test_images_output_improved/solidYellowLeft_grayscale.png)  |  
gaussian_blur:  |   | ![gaussian_blur](test_images_output_improved/solidYellowLeft_gaussian_blur.png)  |  
Canny  |   | ![canny](test_images_output_improved/solidYellowLeft_canny.png)  |  
region of interest:  |   | ![region_of_interest](test_images_output_improved/solidYellowLeft_region_of_interest.png)  |  
hough_lines:  | ![hough_lines](test_images_output/solidYellowLeft_hough_lines.png)  |   |  ![hough_lines](test_images_output_improved/solidYellowLeft_hough_lines.png)
weighted_img:  | ![weighted_img](test_images_output/solidYellowLeft_weighted_img.png)  |   |  ![weighted_img](test_images_output_improved/solidYellowLeft_weighted_img.png)

In order to draw a single line on the left and right lanes, I modified the draw_lines() function by ...

If you'd like to include images to show how the pipeline works, here is how to include an image:

![alt text][image1]


### 2. Identify potential shortcomings with your current pipeline


One potential shortcoming would be what would happen when ...

Another shortcoming could be ...


### 3. Suggest possible improvements to your pipeline

A possible improvement would be to ...

Another potential improvement could be to ...
