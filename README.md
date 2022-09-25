# FCN - Fully Convolutional Networks (Image Segmentation)

Step 1. Building a Network
 
We have used Resnet18 from torchvision as a backbone for initial layers and customised the last layers according to the FCN paper by adding the 1x1 and transposed convolutional layers.

Step 2. Loading dataset

We have used the PASCAL VOC 2012 dataset to train our network that includes 21 classes. The train/val data has 11,530 images containing 27,450 ROI annotated

Step 3. Training

We train our newly constructed fully convolutional network. Because we have predicted the class for each pixel using the output channel of the transposed convolutional layer, the channel dimension is specified in the loss calculation. Furthermore, accuracy is calculated based on the correctness of the predicted class for all pixels.

Step 4. Testing/Prediction

Step 5. Results
