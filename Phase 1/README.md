# Directory structure before running the "CSE515 project phase1.ipynb"
### Start the notebook in the Google colab for smooth run and ignoring the library errors

## Directory structure before running all the cells in the notebook:
```
/
    image-0.png
    test_imgage_sets.zip (Containing set1, set2, set3)
```

# TASK 0
## Familiarizing with the dataset by visualizing the images and printing the shape of the original dataset

# TASK 1
## Implement a program which, given an image ID and one of the following models, extracts and prints (in a human readable form) the corresponding feature descriptors: Color moments, Standard deviation and Histogram of oriented gradients.
### There are 3 main functions for 3 models (Color moments, Extended local binary patterns, Histogram oriented gradients) namely, ColorMoments, localBinPattern, histOrientedGrad.
### Input to these functions: A single array containing array(s) of image(s)
### Output: Array comprising features of the image(s)

### TASK1 Final function:
### Inputs: Path of the image, model function
### Output: A .txt file containing the features of the image calculated by the model passed in parameter

# TASK 2
## Implement a program which, given a folder with images, extracts and stores feature descriptors for all the images in the folder.
### TASK2 Final function:
### Inputs: An array containing the lists of the images in each subfolder (Shape of this array will be (m, ) for a folder containing m subfolders, each of this 3 arrays/lists have shape of (n, 64, 64) where n=number of images in that subfolder)
### Output: Text files containing the feature descriptors of the images for the m sets(subfolders) for all 3 models are created in each subfolder.

# TASK 3
## Implement a program which, given a folder with images and an image ID, a model, and a value “k”, returns and visualizes the most similar k images based on the corresponding visual descriptors. For each match, also list the overall matching score.
### TASK3 Final function:
### Inputs: Folder path containing the subfolders containing the images, Name of the image to be compared, Model function, Value of k
### Output: Each subfolder in the folder will have 3 text files namely, TASK3KNearestColorMoments.txt, TASK3KNearesthistOrientedGrad.txt, TASK3KNearestlocalBinPattern.txt comprising the names of the k-nearest images and their respective distances with the base image.

# TASK 4
## Implement a program which, given a folder with images and an image ID and a value “k”, returns and visualizes the most similar k images based on all corresponding visual descriptors. For each match, also list the overall matching score and the contributions of the individual visual models.
### TASK4 Final function:
### Inputs: Folder path containing the subfolders containing the images, Name of the image to be compared, Model function, Value of k
### Output: Each subfolder in the folder will have 3 text files named TASK4outputFeatures.txt comprising the names of the k-nearest images and their respective distances with the base image.

## Directory structure after running all the cells in the notebook:
```
/
    TASK1.txt
    image-0.png
    test_imgage_sets.zip
    images/
        set1/
            TASK3KNearestlocalBinPattern.txt
            TASK2outputFeatures.txt
            TASK3KNearestColorMoments.txt
            image-2.png
            TASK4outputFeatures.txt
            image-9.png
            image-8.png
            image-7.png
            image-0.png
            image-6.png
            image-4.png
            image-1.png
            image-3.png
            image-5.png
            TASK3KNearesthistOrientedGrad.txt
        set2/
            TASK3KNearestlocalBinPattern.txt
            TASK2outputFeatures.txt
            TASK3KNearestColorMoments.txt
            image-12.png
            image-10.png
            image-2.png
            TASK4outputFeatures.txt
            image-11.png
            image-0.png
            image-4.png
            image-1.png
            image-13.png
            image-3.png
            image-14.png
            TASK3KNearesthistOrientedGrad.txt
        set3/
            TASK3KNearestlocalBinPattern.txt
            image-60.png
            TASK2outputFeatures.txt
            TASK3KNearestColorMoments.txt
            image-110.png
            image-10.png
            image-40.png
            TASK4outputFeatures.txt
            image-80.png
            image-100.png
            image-0.png
            image-70.png
            image-120.png
            image-90.png
            image-50.png
            image-30.png
            TASK3KNearesthistOrientedGrad.txt
            image-130.png

```
