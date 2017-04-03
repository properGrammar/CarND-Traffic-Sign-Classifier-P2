
## PROJECT SPECIFICATION: Traffic Sign Classifier

Project 2 for the Udacity Self-Driving Car Nanodegree, January 2017 Cohort

by Graham Arthur Mackenzie

Nota Bene: Rather than put all the verbiage here and all the code over there, for ease of reading / comprehension of my process, I have put both over there and just used this writeup as a rubric criteria checklist, so to speak. I hope my formatting here is self-explanatory, but just in case it's not: Look at the cell numbers in the parentheses prior to every MEETS SPECIFICATIONS to see where in GAM_Traffic_Sign_Classifier.ipynb you can find the requisite code. Cheers!

- - -

CATEGORY: Files Submitted

CRITERION: Submission Files

(see submitted files) MEETS SPECIFICATIONS: The project submission includes all required files. Namely: 
- The Traffic_Sign_Classifier.ipynb notebook file with all questions answered and all code cells executed and displaying output.
- An HTML or PDF export of the project notebook with the name report.html or report.pdf.
- Any additional datasets or images used for the project that are not from the German Traffic Sign Dataset. Please do not include the project data set provided in the traffic-sign-data.zip file.
- Your writeup report as a markdown or pdf file

- - - 

CATEGORY: Dataset Exploration

CRITERION: Dataset Summary 

(cell 2) MEETS SPECIFICATIONS: The submission includes a basic summary of the data set.

CRITERION: Exploratory Visualization

(cells 3 + 4) MEETS SPECIFICATIONS: The submission includes an exploratory visualization on the dataset.

- - -

CATEGORY: Design and Test a Model Architecture

CRITERION: Preprocessing

(cells 5 - 8) MEETS SPECIFICATIONS: The submission describes the preprocessing techniques used and why these techniques were chosen.

CRITERION: Model Architecture

(cells 9 + 10, and then again at 12 + 13) MEETS SPECIFICATIONS: The submission provides details of the characteristics and qualities of the architecture, such as the type of model used, the number of layers, the size of each layer. Visualizations emphasizing particular qualities of the architecture are encouraged.  

CRITERION: Model Training

(cell 11) MEETS SPECIFICATIONS: The submission describes how the model was trained by discussing what optimizer was used, batch size, number of epochs and values for hyperparameters.

CRITERION: Solution Approach

(cell 12) MEETS SPECIFICATIONS: The submission describes the approach to finding a solution. Accuracy on the validation set is 0.93 or greater.

- - -

CATEGORY: Test a Model on New Images

CRITERION: Acquiring New Images

(cells 29 + 30) MEETS SPECIFICATIONS: The submission includes five new German Traffic signs found on the web, and the images are visualized. Discussion is made as to any particular qualities of the images or traffic signs in the images that may be of interest, such as whether they would be difficult for the model to classify.

CRITERION: Performance on New Images

(cell 33) MEETS SPECIFICATIONS: The submission documents the performance of the model when tested on the captured images. The performance on the new images is compared to the accuracy results of the test set.

CRITERION: Model Certainty - Softmax Probabilities

(cells 33 + 34) MEETS SPECIFICATIONS: The top five softmax probabilities of the predictions on the captured images are outputted. The submission discusses how certain or uncertain the model is of its predictions.

- - -

CATEGORY: Suggestions to Make Your Project Stand Out! Here are a few ideas for going beyond the requirements outlined in the rubric.

CRITERION: Augment the Training Data

(cells 14 - 27) MEETS SPECIFICATION: Augmenting the training set might help improve model performance. Common data augmentation techniques include rotation, translation, zoom, flips, and/or color perturbation. These techniques can be used individually or combined.

CRITERION: Analyze New Image Performance in More Detail

(cells 35 + 36) MEETS SPECIFICATION: Calculating the accuracy on these five German traffic sign images found on the web might not give a comprehensive overview of how well the model is performing. Consider ways to do a more detailed analysis of model performance by looking at predictions in more detail. For example, calculate the precision and recall for each traffic sign type from the test set and then compare performance on these five new images..
	If one of the new images is a stop sign but was predicted to be a bumpy road sign, then we might expect a low recall for stop signs. In other words, the model has trouble predicting on stop signs. If one of the new images is a 100 km/h sign but was predicted to be a stop sign, we might expect precision to be low for stop signs. In other words, if the model says something is a stop sign, we're not very sure that it really is a stop sign.
	Looking at performance of individual sign types can help guide how to better augment the data set or how to fine tune the model.

CRITERION: Create Visualizations of the Softmax Probabilities

(cell 33) MEETS SPECIFICATION: For each of the five new images, create a graphic visualization of the soft-max probabilities. Bar charts might work well.

CRITERION: Visualize Layers of the Neural Network

(incomplete) MEETS SPECIFICATION: Deploy outputFeatureMap() to visualize your network's feature maps.
	NVIDIA (for example) was able to show that their network's inner weights had high activations to road boundary lines by comparing feature maps from an image with a clear path to one without. Try experimenting with a similar test to show that your trained network's weights are looking for interesting features, whether it's looking at differences in feature maps from images with or without a sign, or even what feature maps look like in a trained network vs a completely untrained one on the same sign image.
	Discuss how you used the visual output of your trained network's feature maps to show that it had learned to look for interesting characteristics in traffic sign images. 
