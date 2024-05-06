# ASLClassification
ASL Recognition using classification methods

The goal of this project is to recognize ASL signs from a given video based on coordinate locations and hand positioning and facial movement. 

First, the videos must be processed into x,y,z coordinate locations using the demoPoseEstimationforVideoFolders file. In this file, edit the path of the folder that contains the training mp4 videos to reflect your path. Included, is a folder called book-drink-videos that contains videos for book and drink. This should output the processed csv's into a specified folder (edit this path to adjust output folder location). (*Note that there is already preprocessed csv's for the mp4 files in the asl-csv data, which includes training csv as well as testing ones. This step can be skipped if asl-csv-data is used as input for model training.)

Second, once the csv files are created, to train the models on the csv data, edit the folder path in the first cell block (in files Sign-Identification-With-Random-Forests, Sign-Identification-With-LogisticRegression, and Sign-Identification-With-Clustering) to reflect the name and path of your csv data folder. 

Then, in the last block, adjust the path of the testing files to reflect yours. (Testing files are included in asl-csv-data/book_drink_test). 
