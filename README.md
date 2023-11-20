# Pistachio Image Classification : Project Overview
* Developed a pistachio image recognition model to aid in identifying different varieties of pistachios, facilitating sales.  
* Utilized deep learning techniques to implement a convolutional neural network to build the model.  
* Employed transfer learning techniques, including VGG16, MobileNet, and EfficientNet, to optimize models, achieving an accuracy rate of 98.8%.
* Provide detailed explanations of my thought process and how to make adjustments to the model.  
 
 ## Let's get started!
 **Hello everyone, in this notebook, I will be utilizing transfer learning to build our model. I've fine-tuned a model based on data, and throughout the model-building process, I will provide detailed explanations of my thought process and how to make adjustments to the model.**  
 > ### Here's the outline of this notebook  
1. [Import Library](#item1)
2. [Data Preprocessing](#item2)  
3. [EDA](#item3)  
4. [Image Generator](#item4)  
5. [Create CNN model](#item5)  
6. [Create VGG16 model](#item6)  
7. [Create MobileNet model](#item7)  
8. [Create EfficientNet model](#item8)  
9. [Predict and Evaluate Model with Data Visualization](#item9)
  
**I will focus on introducing the dataset, the performance of MobileNet, and the final prediction results. If you would like to see more detailed content, please feel free to check out the notebook.**  
## First, Let's explore dataset.  
**This dataset consists of two types of pistachios: Kirmizi and Siirt. Let's take a look at their distribution.**  
![download](https://github.com/Elvis-YAL/Pistachio-Image-Classification/assets/40426433/bc515c59-694a-4306-ad20-5070585c117b)

 **Next, let's take a look at the images in this dataset.**  
 
![download](https://github.com/Elvis-YAL/Pistachio-Image-Classification/assets/40426433/99a38e7a-ce72-4a3b-b0aa-499ec3d67214)

**Next, I applied data augmentation to the images to enhance the learning process with different perspectives of the data.**  
![download](https://github.com/Elvis-YAL/Pistachio-Image-Classification/assets/40426433/1253faa5-69b3-4f8b-82b0-eae0e366f48f)

## Let's create our MobileNet Model  
In this model, I conducted some fine-tuning, including adjusting the learning rate, tuning the number of dense neurons, experimenting with l1_l2 regularization, and modifying the patience and epoch count for early stopping.  
**Ultimately, it achieved an excellent accuracy of 0.98.**  
Let's take a look at how it performs in terms of loss and accuracy.  
![download](https://github.com/Elvis-YAL/Pistachio-Image-Classification/assets/40426433/4301add6-6525-4a21-90cc-285c8c8478de)

**And present the entire architecture of the model.**   
![download](https://github.com/Elvis-YAL/Pistachio-Image-Classification/assets/40426433/97084808-4160-430f-9a0e-11d076982bf8)

**In the end, I randomly selected 16 images from the test set and labeled them with their original classes and predicted classes as titles. It's evident that almost all the predictions are quite accurate.**  
![download](https://github.com/Elvis-YAL/Pistachio-Image-Classification/assets/40426433/d7f1657c-be54-4d99-bdf3-f8952486a781)



