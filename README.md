# Emotion-Detection

This project's main objective is to build a model that will classify emotions in five different categories: Angry, Happy, Sad, Surprise, and Neutral. However, many complex models are available to use, provided by AWS or Google cloud services. Although this project's scope is limited to recognizing seven expressions, this can be further expanded to the practical use of video games where players are engaged with game characters and their movement is followed by characters. There are vast domains where real-time emotion detection is beneficial to improve services for users.

For implementing all the features of application, Python, Keras, and OpenCV was used.

Task 1: Import the modules that are needed for this project. These are the project's wheels. This may also require installing some libraries before importing them.

Task 2: Collect the data from dataset available online. For this project, dataset was downloaded from the Kaggle website. The dataset totally contains 7 classes of emotions namely Sad, Happy, Angry, Fear, Disgust, Surprised and Neutral. For the scope of this project only 5 classes were used for training and validation. The data in the dataset is segregated in 5 different folders.

Task3: Image augmentation is used on the database. Image Data Augmentation is a technique for artificially increasing the size of a training dataset by generating updated versions of the images in the dataset. The ImageDataGenerator class in the Keras deep learning neural network library allows you to fit models using image data augmentation.

Task 4: After the dataset modification is complete, next task is to develop the brains of the whole application i.e., the CNN. A sequential model is used which typically defines how model will have layers one after another.

<img width="663" alt="Screen Shot 2021-04-28 at 6 49 49 PM" src="https://user-images.githubusercontent.com/32639884/118729561-fffe0580-b7ea-11eb-8700-419ed0415e4b.png">
<img width="524" alt="Screen Shot 2021-04-28 at 6 50 46 PM" src="https://user-images.githubusercontent.com/32639884/118729569-02605f80-b7eb-11eb-8e34-2734dd67459f.png">

Task 5:
Compile the model and save. But there are various things to do before compiling.
• Checkpoint: It will monitor the validation loss and will try to minimize the loss using the
mode=’min’ property. When the checkpoint is reached it will save the best trained
weights.

• Early Stopping: This will stop the execution by monitoring different properties such as monitor,
min_delta (minimum change in monitored quality), verbose. Etc.

• Reduce Learning rate: When learning becomes stagnant, models also benefit from reducing the learning rate by a factor of 2–10. This callback measures a quantity, and if there is no change after a certain number of epochs, the learning rate is decreased.

Then just configure two functions of compiling model and fitting the model in desired object.
![Screen Shot 2021-04-29 at 1 36 16 PM](https://user-images.githubusercontent.com/32639884/118729622-173cf300-b7eb-11eb-8678-cf982cce0166.png)
