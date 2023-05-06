# CS598-DLH : Patient-Phenotyping
## Patient Phenotyping
This repository contains the code and data to create CNN based classifier for Patient Phenotyping.

### Data

1. Patient Notes Data - This file is too large to upload into GitHub. The file can be downloaded from following location - https://physionet.org/content/mimiciii/1.4/ 
3. Annotations - This file contains the annoations on 1670 patients data. The file is present in Data folder.
4. Final File - This file has been created by merging the patient notes and annotation data. Only records for the matching patients in both the files have been kept. This is the file used to train/ validate/ test the CNN model.
5. If one wants to start the process from scratch. please download the data from the above address and run the pre-process code to create the final file.
6. We also provide a file called dataset_dict.pickle which already contains the train/ test and validation data split. 
 
### Code
1. Pre_processing - This file provides the code to read, merge and join the patient notes and annotations. If the patient notes file can be availed, then place the file along with the annotations file and run the code. This is a google colab notebook. To use the notebook, please create folders in google drive and place the files in the appropriate folders. 

The final file has aready been given and the Pre-Processing step can be skipped.

DLH_Patient_Phenotyping.ipynb - This google colab notebook does the following -
  * Reads the final file
  * Cleans the text data
  * Create a CNN Classifier
  * Trains the Model
  * Evaluates the model

To run this, please use google colab. Place the final file in the fodler suggested

2. 
  
### Model
A pretrained model has been provided. The pretarined model can be loaded directly instead of training the mode from scratch. All one has to do is to take the final_files.csv and create a sample test data. Load and evaluate model using the test data.



## References
<a id="1">[1]</a> 
Gehrmann S, Dernoncourt F, Li Y, Carlson ET, Wu JT, Welt J, Foote J Jr, Moseley ET, Grant DW, Tyler PD, Celi LA. Comparing deep learning and concept extraction based methods for patient phenotyping from clinical narratives. PLoS One. 2018 Feb 15;13(2):e0192360. doi: 10.1371/journal.pone.0192360. PMID: 29447188; PMCID: PMC5813927.


### Note :
Below is the code base for the paper listed under reference.
https://www.cs.cornell.edu/courses/cs4780/2018fa/lectures/lecturenote17.html
