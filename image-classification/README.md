# Project 2: Image Classification
In this project, the CIFAR-10 dataset is used. The dataset consists of airplanes, dogs, cats, and other objects. The dataset will need to be preprocessed, then train a convolutional neural network on all the samples. You'll normalize the images, one-hot encode the labels, build a convolutional layer, max pool layer, and fully connected layer. At then end, you'll see their predictions on the sample images.

This project runs on [floydhub.com](https://www.floydhub.com)

floyd tutorial can be found in [this site](https://github.com/ludwiktrammer/deep-learning/tree/master/image-classification)

1. Install the `floyd` command on your computer:

        pip install -U floyd-cli
        
    Do this even if you already installed `floyd-cli` before, just to make sure you have the most recent version (its peace of development is fast!).

2. Associate the command with your Floyd account:

        floyd login

3. Clone this repository:

        git clone https://github.com/ludwiktrammer/deep-learning.git

4. Enter the folder for the image classification project:

        cd image-classification

5. Initiate a Floyd project:

        floyd init dlnd_image_classification

6. Run the project:

        floyd run --gpu --env tensorflow --mode jupyter --data diSgciLH4WA7HpcHNasP9j

    It will be run on a machine with GPU (`--gpu`), using a Tenserflow environment (`--env tensorflow`), as a Jupyter notebook (`--mode jupyter`), with Floyd's built-in cifar-10 dataset  available (`--data diSgciLH4WA7HpcHNasP9j`).
    
7. Wait for the Jupyter notebook to become available and then access the URL displayed in the terminal (described as "path to jupyter notebook"). You will see the notebook.

8. Remember to explicitly stop the experiment when you are not using the notebook.

        floyd stop ID   

9. If you already stoped the experiment, you can still download the file using the `floyd output` command:

    floyd output ID