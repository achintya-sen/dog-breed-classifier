[//]: # (Image References)

[image1]: ./images/Picture3.png "Sample Output 1"
[image2]: ./images/Image1.png "Sample Output 2"
[image3]: ./images/Picture1.png "Sample Output 3"
[image4]: ./images/Picture2.png "Sample Output 4"


## Project Overview

The dog breed classifier project is well known in the Computer Vision domain. The first competition for this was first raised in Kaggle in 2017 (Kaggle, n.d.), where the primary objective was to distinguish the breed of a dog given an input image. As the primary objective of this project, I would be building an interface through which an image can be pushed into a data pipeline to pass into a Convolutional Neural Network (CNN) which will output the breed of the input image. There are many types of breeds against the dataset, which makes it a multi-class classification problem.   

![Sample Output 1][image1]

A fun aspect of this project is to input images of humans and see the breed against which they match the most. The interface would take as input any image a run pre-trained model to classify a human for breed classification based on the model.

![Sample Output 2][image2]


## Project Instructions

### Instructions

1. Clone the repository.
2. Download the [dog dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/dogImages.zip).  Unzip the folder and place it in the repo, at location `path/to/dog-project/dogImages`.  The `dogImages/` folder should contain 133 folders, each corresponding to a different dog breed.
3. Download the [human dataset](http://vis-www.cs.umass.edu/lfw/lfw.tgz).  Unzip the folder and place it in the repo, at location `path/to/dog-project/lfw`.  If you are using a Windows machine, you are encouraged to use [7zip](http://www.7-zip.org/) to extract the folder. 
4. Make sure you have already installed the necessary Python packages according to the `requirement.txt` file in the program repository.
    ```
		pip install -r requirement.txt
	```
5. Open a terminal window and navigate to the project folder. Open the notebook and follow the instructions.
	
	```
		jupyter notebook dog_app.ipynb
	```
6. Execute the notebook by selecting Cells -> Run All
7. Please be advised the aforementioned process with generate the model_artifacts needed for execution.
8. At the bottom of the notebook specify the the image path as follows:
    ```python
    run_app("my_dog_image.png")
	```
  ![Sample Output 3][image3]

Or you can enter human image and see the result.

   ```python
   run_app("my_human_image.png")
   ```
	
  ![Sample Output 4][image4]


__NOTE:__ In the notebook, you will need to train CNNs in PyTorch.  If your CNN is taking too long to train, feel free to pursue one of the options under the section __Accelerating the Training Process__ below.

## (Optionally) Accelerating the Training Process 

If your code is taking too long to run, you will need to either reduce the complexity of your chosen CNN architecture or switch to running your code on a GPU.  If you'd like to use a GPU, you can spin up an instance of your own.
