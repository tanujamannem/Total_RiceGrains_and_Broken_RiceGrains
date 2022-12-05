# Total_RiceGrains_and_Broken_RiceGrains
**Counting Rice Grains**

**Objective 1:** Count the number of rice grains in the Image.

**Objective 2:** Find the number of broken grains in the image.

You can assume the following in the image:

● The background will always be blue.

● There will be a mix of broken and non-broken rice grains.

● The grains will not overlap but can touch each other.

**Technology used:** Computer Vision, OpenCv, WaterShed-Algorithm, Image Segmentation, Image Pre-processing.

**Approach for the Solution:**

1. Importing Required libraries

2. Defining show Function for image visualization

3. Image Pre-Processing

4. Counting Rice grains using Contours Method

5. Solving Grains touching problem by using watershed Algorithm

6. Counting total rice grains and total broken rice grains using contour area

**Explanation of total process:**  The main objective of this task is to count the total number of rice grains and total number of broken rice grains in given images.

--> Loaded the image file by using show method for that created function.For counting the rice grains, to solve the pre processing of the image. There are mainly two tasks in this.

1. Image Pre Processing

2. Solving grains touch problem

**1. Image Pre Processing:** Image processing is playing key role for getting image clear.The difficult part of Image preprocessing is tuning the Image, it takes a lot of trail and error to fix the parameter to the required value.In this, There are three major steps.

<1> Converted colour image to greyscale image.

<2> Image Thresholding

<3> Removing the noise from the image by using MorphologyEx.

After all these steps, got clear image for next process.

**2. Solving grains touch problem:** The next step is to count the rice grains that are touching each other.

--> It is difficult to count manually. For Machines, counting rice grains are very easy if they are separated. For small size rice grains, It becomes more difficult.

--> For that I applied Watershed Algorithm. Watershed algorithm extracts based on the background and it detects the edges of the rice grains.

**Conclusion:** Finally, got total number of rice grains present in the image but counting the broken rice grains is typical task. For that, I used area based approach. If the area of the image is below to the threshold then it is broken rice grain.
So, calculated total rice grains and broken rice grains.
