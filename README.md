🎯Problem Statement: Identify the dog breed from the image using machine Learning Principles.
✒️Machine Learning Principle Used: Transfer Learning, Neural Network.
🔨⛏️Library used: Tensorflow, Tensorflow Hub, Scikit Learn, Numpy, Pandas, Matplotlib, Seaborn, Os.

💥Major steps:
1️⃣ EDA [Exploratory Data Analysis]:
>> Checking and understanding the provided dataset helps with the help of graphs. Check if the data set has enough images per class to be classified if any given column has empty rows, and if we have class imbalance using numpy, pandas, and matplotlib.
2️⃣ Pre-processing images and labels:
>>converted the given filename into proper file paths and converted labels(breeds) to Boolean and binary value arrays. Converted the images into tensors to make them compatible with TensorFlow. 
3️⃣ Modelling:
>> Various User-defined functions to split data into batches and visualize them were made to ease our workflow.
>>Since the Validation set was not provided, I created a validation set with an 80 -20 split on the training set.
>> Callbacks were made, namely, for early stops and TensorFlow Hub.
>>Created a Neural Network using Sequential API and mobilenet_v2_130_224 layer from the tfhub ..and adjusted the output layer using SoftMax activation.
>>Later the model was Trained on the complete data set of 10,000+ images.
4️⃣ Saving  & Reloading :
>> Every model is saved with a proper timestamp for future use and compared with future improvements.
>> Further, these models can be shared with others and ready to be deployed.
5️⃣ Making Prediction.
>> The test data set was imported explicitly, and predictions were made.
>>Later, I converted the predictions into CSV of the desired form to be submitted at Kaggle.
6️⃣ Custom Images:
>> Why shouldn't I use my project for fun... I can now upload my own clicked images and boom 💥, I will get to know the breed of the dog.
