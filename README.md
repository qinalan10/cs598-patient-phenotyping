# CS598-DLH : Patient-Phenotyping
## Patient Phenotyping
This repository contains the code and data to create CNN based classifier for Patient Phenotyping.
### Data
1. Patient Notes Data - This file is too large to upload into gihub. 
2. Annotations - This file contains the annoations on 1670 patients data. The 
3. Final File - This file has been created by merging the patient notes and annotation data. Only records for the matching patinets in both the files have been kept. This is the file that is used to train the CNN model.
### Code
1. Pre_processing - This file provides the code to read, merge and join the patient notes and annotations. If the patient notes file can be availed, then place the file along with the annotations file and run the code. This is a google colab notebook. To use the notebook, please create folders in google drive and place the files in the corresponding folders. 

2. DLH_Patient_Phenotyping.ipynb - This google colab notebook does the following -
  asdad
  adasda

### Model
A pretrained model has been provided. The pretarined model can be loaded directly instead of training the mode from scratch. All one has to do is to take the final_files.csv and create a sample test data. Load and evaluate model using the test data.
