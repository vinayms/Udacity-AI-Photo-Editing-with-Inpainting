# Udacity-AI-Photo-Editing-with-Inpainting
Project to show how Generative Models can be used in Computer Vision

### Project Overview
## Project Introduction
In this class we have seen how Generative models can be used in Computer Vision. We have also seen how to use the Segment Anything Model to select subjects in images by providing points and other inputs.

Let's put some of this knowledge to good use by building something interesting, and fun!

A screenshot of the app we are going to build, showing how we can substitute the background of a subject with a computer-generated one described through text
With our app we will be able to swap out the background of an image and substitute it with a computer-generated one described through text

An image of a cat is shown, with green points marking input points for the Segment Anything Model (SAM). SAM returns a segmentation mask, then through a text prompt the cat is removed and an crocodile is put in its place.
We can also substitute the subject instead of the background

Project Summary
In this project we are going to build a little app that allows you to select a subject and then change its background, OR keep the background and change the subject.

The process involves a user uploading an image and selecting the main object by clicking on it. The Segment Anything Model (SAM) is activated to create a mask around the selected object, choosing the most accurate mask generated. The user is shown this result to either accept it or refine the mask further with additional points. Once the mask is finalized, the user gives a text description (and possibly a negative prompt) to specify a new background for the selected object. An infill model then creates this new background, and the final image is displayed. Optionally, the user can choose to invert the mask and substitute the subject while keeping the background, as in the example above.

This little app can be used to swap backgrounds, swap subjects, remove objects, and more!

You will be writing the code that powers the main functionality of the app: calling the SAM model and processing its output, as well as using a text2image diffusion model to generate the new background or subject.

## Sample

![alt text](https://github.com/vinayms/Udacity-AI-Photo-Editing-with-Inpainting/edit/main/daenerys_walking_in_starbucks.PNG)


![alt text](https://github.com/vinayms/Udacity-AI-Photo-Editing-with-Inpainting/edit/main/tyrion_in_new_york_city.PNG)


