# **Finding Lane Lines on the Road**

## Lane Finding: It came together like a jig

---

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report


[//]: # (Image References)

[image1]: ./examples/grayscale.jpg "Grayscale"

---

### Reflection

### 1. Basic Pipeline for Finding Lanes

I followed all of the basic steps outlined in the lessons.
`line_finding_pipeline` is me adding to each step (or pass)
I found when reviewing the lessons on what to do next. First, I do a simple greyscale. Then, I filter out the triangle area I want to search. Next, Canay image processing
is done with the parameters mentioned in the lessons. Finally, we do Hough transformations.

The only post processing I do is merging the lines to the original image.

![alt text][image1]


### 2. Identify potential shortcomings with your current pipeline

I fail the challenge. I have no  idea why the image is so
crazy shaped but I ran out of time before finding improvements. I think the reflections of the dashboard is being picked up by the line drawing algorithm, too.

The lines I find are not actually lining up exactly with the lane markers, too.

### 3. Suggest possible improvements to your pipeline

I definitely want to tighten up the lines and pass the challenge.

For the challenge to pass, I think I might have to create a way to line up the steering wheel with the polygon filter that renders on the screen. If I turn the wheel harder in one direction, the resulting polygon will start to curve and lean in that direction.
