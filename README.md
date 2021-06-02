# COVID-19-Detection-Using-CNN-and-Transfer-Learning-InceptionV3-ResNet50-VGG16

Deep learning has applied in various domains such as energy, finance, and the medical field. In this project, we applied deep learning for COVID-19 detection. We have applied four different deep learning models: CNN model, CNN model with regularization, CNN model with Image augmentation and Transfer learning model (InceptionV3, ResNet50, VGG16) with image augmentation.

We have built a basic CNN model with three convolutional layers coupled with max-pooling for feature extraction and downsampling the output convolution feature maps. Then, we tried to improve the model with regularization by adding a dropout of 0.3 after each hidden layers. We also applied Image augmentation with our CNN model by applying image transformations like rotation,  shearing, zooming to produce a new version of the image. Finally, we used a pre-trained transfer learning model like InceptionV3, VGG16 and RestNet50, where we freeze all the network layers to fix their model parameters. We have trained all the model with a batch size of 32 and 30 epochs.

COVID-19 Chest X-ray radiography images databases from the Kaggle repository (https://www.kaggle.com/tawsifurrahman/covid19-radiography-database) are taken. The dataset consists of Chest X-ray images for COVID-19 positive cases patients 2295 patients with 1583 normal images and 712 covid images. Out of these, 1811 chest x-ray images are used for training (1266 Normal/545 COVID) and 484 images are used for testing (317 Normal/167 COVID).  

Our results showed that the basic CNN model has overfitting based on training/validation accuracy/losses.  We also noticed overfitting had been slightly reduced in the CNN model with regularization.  For image augmentation with our CNN model, we observed that overfitting had been dramatically reduced. We noticed that their results are pretty similar to our CNN model with the image augmentation method for transfer learning.

Future Works
1.	Transfer learning will be used for feature extraction, and the output of corresponding transfer learning will be feed to our CNN model
2.	Freezing only some of the network layers of transfer learning and fine-tuning the remaining network layers of transfer learning along with our CNN model.
