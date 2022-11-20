#### ResearchProject

## Model_To_Train folder contains : 

Text_Classification_Model.ipynb: It is a Google-Colab notebook with comments explaining the working of the various cells.
Dataset: a subfolder containing the formatted OPP-115 dataset for training.

Steps to execute the training model:
1.	Download the file 'Text_Classification_Model.ipynb' (notebook1) and the dataset file.
2.	Upload the dataset file to Google Drive.
3.	Open notebook1 in a browser.
4.	Notebook1 has a cell that would mount the Google Drive to the notebook’s environment.
5.	Change the path name in the variables:
    trainPath: path of the file train_dataset.csv
    valPath = path of the file validation_dataset.csv"
    tDFPath = path to save the train dataframe
    valDFPath = path to save the validation dataframe
6.	The execute cells one by one. 

__________________________________________________________________________________________________________________________________________________________________
## PrivacyInterpreterM.ipynb : PolicyInterpreter scrapes the privacy policy from a given URL and then according to the user type selected classifies the policy into privacy categories and then using cosine similarity selects similar sentences to form a summary.

Steps to execute the proof-of-concept model
1.	Download “PolicyInterpreterM.ipynb” (notebook2), the configuration files present in the “Model_Configuration” folder.
2.	Upload the selected configuration into Google Drive.
3.	Notebook2 has a cell that would mount Google Drive to the notebook environment.
4.	Change the path in the variable 'modelDir' to the path where the configuration is saved. 
5.	Execute each cell one by one. The initial cells contain the important libraries that need to be included. Run all the cells until the Main section. 
6.	The Main section provides a place to input the user type and URL of the privacy policy.
7.	During the first run of the notebook, the libraries and checkout points are downloaded. Therefore, certain cells would take longer to execute. Once the     libraries are cached, the cells run normally. 
____________________________________________________________________________________________________________________________________________________________________
Note
1. This is only a proof-of-concept model of PrivacyInterpreter.
2. It is highly recommended to use the GPU provided by Google-Colab to train the model. Running the training algorithm requires a lot of RAM and the program        crashed when all the available RAM is consumed. Instead of mounting the Google drive, the required files could be uploaded to the session storage. But this upload  or saving of the file would be lost when the session is closed.

