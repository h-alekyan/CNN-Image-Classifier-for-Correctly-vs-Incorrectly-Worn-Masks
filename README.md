# Convolutional Neural Network Image Classifier for Correctly vs Incorrectly Worn Masks
Convolutional Neural Network Image Classifier for Correctly vs Incorrectly Worn Masks

# Method
Preprocessed the data by categorizing them as 0 or 1 as correctly worn or incorrectly worn respectively. I also grayscaled the images to save memory and increase performance efficeincy. Then use pickle to store the preprocessed data as arrays. I would **not recommend** using pickle in general, this was just a quick solution since I had a small dataset at hand and was not concerned with speed issues. 
Using a simple CNN with 2 conv2d layers + flatten and dense layers. As for the optimizer, I went for the popular option and chose adam. SGD would also work, but I would have to manually give more parameters, which is avoided by choosing adam.  

# Dataset
The primary source of the image data was https://github.com/cabani/MaskedFace-Net
I was not using AWS and it would take time to get p2.xlarge instances and I wanted to finish this project in a shorter period of time.

# Future improvements
You are free to use the code and here are some possible improvement suggestions:
- instead of using imgread use cv2 to record live camera performance and tell whether the mask is worn correctly or not.
