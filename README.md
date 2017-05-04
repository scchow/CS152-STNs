# CS152-STNs

This page contains the code used for testing the Spatial Transformer Network.


## Folders

[`docs`](docs) folder contains the webpages used to host the project website.
[`output`](output) folder contains the output of various tests.
[`stn_code`](stn_code) folder contains the code used to run the multiple tests.
[`stn_code\data`](stn_code\data) consists of the mnist data set in an `.npz` file.

## Files
[`data_compilation.xlsx`](data_compilation.xlsx) contains the plotted data of the results
[`run.bat`](run.bat) contains a script containing sample commands to run the files. 
Note: Running the bat file by itself has not been tested. Use the file by copying and pasting onto the command line. Also command line arguments are Windows only.
[`STN_paper_better.pdf`](STN_paper_better.pdf) is the main paper on Spatial Transformer Networks, copied to the repository for convenience.
[`useful_regex.txt`](useful_regex.txt) contains several regex that are useful for parsing output files. They are included for reference.

## Main Code
Code is contained with [`stn_code`](stn_code).

Each of the following python scripts takes in two parameters. 
- The first input is the run number that will be appended to the output files for sorting. 
- The second input is the number of epochs to run the test.

[`cluttered_mnist_cnn_only.py`](stn_code\cluttered_mnist_cnn_only.py) will try to identify the cluttered MNIST dataset with only the Convolutional Neural Network (CNN).
[`cluttered_mnist_stn.py`](stn_code\cluttered_mnist_stn.py) will try to identify the cluttered MNIST dataset by running the data through the Spatial Transformer (ST) before the CNN.
[`cluttered_mnist_multistn.py`](stn_code\cluttered_mnist_multistn.py) will try to identify the cluttered MNIST dataset with an ST before the CNN and an ST layer between the 1st and 2nd layers of the CNN.
For details of the ST and CNN setup, see our [project website](https://scchow.github.io/CS152-STNs/index.html).

