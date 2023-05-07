# CS598-DLH : Patient-Phenotyping
## Patient Phenotyping

This repository contains the code and data to create CNN based classifier for Patient Phenotyping. 

### Data

The data used for this experiment is present in MIMIC-III database. 

1. Patient Notes Data - This file is too large to upload into GitHub. The file can be downloaded from following location - https://physionet.org/content/mimiciii/1.4/. Additonally, this data is sensitive and shouldn't be uploaded in public forum.
2. Annotations - This file contains the annoations on 1670 patients data. The file is present in Data folder.
3. Final File - This file has been created by merging the patient notes and annotation data. Only records for the matching patients in both the files have been kept. This is the file used to train/ validate/ test the CNN model.
4. If one wants to start the process from scratch. please download the patients' notes data from the above address and run the pre-process code to create the final file.
5. We also provide a file called dataset_dict.pickle which already contains the train/ test and validation data split. 
 
### Code
1. Pre_processing - Data_Pre_Processing.ipynb - This file provides the code to read, merge and join the patient notes and annotations. If the patient notes file can be availed, then place the file along with the annotations file and run the code. This is a google colab notebook. To use the notebook, please create folders in google drive and place the files in the appropriate folders and run. 

The final file has aready been given and the Pre-Processing step can be skipped if needed.

2. CNN Model - DLH_Patient_Phenotyping_final.ipynb.ipynb - This google colab notebook does the following -
  * Reads the final file
  * Cleans the text data
  * Creates Word Embeddings
  * Create a CNN Classifier
  * Trains the Model
  * Evaluates the model
  * Results of the model evaluation

To run this, please use google colab. Place the final file in the folder suggested and run.

### Model
A pretrained model has also been provided in /Model folder. The pretarined model can be loaded directly instead of training the mode from scratch whihc is time consuming. The test data has been loaded into a pickle file. Please load the test data from the pickle file suggested in the data section and run the notebook - DLH_Patient_Phenotyping_Model.ipynb. The test data is exactly the same test data that is created in the original model building file. So, this should produce the exact results as the orignal file.

### Experiments
We have run multiple experiments on top of the final model that we were able to compile. The experiments are supplied as their own colab notebook files and is present at Code/Experiments folder.

There are 5 experiments performed and the results and updated parameters are present in the same notebook.

## References
<a id="1">[1]</a> 
Gehrmann S, Dernoncourt F, Li Y, Carlson ET, Wu JT, Welt J, Foote J Jr, Moseley ET, Grant DW, Tyler PD, Celi LA. Comparing deep learning and concept extraction based methods for patient phenotyping from clinical narratives. PLoS One. 2018 Feb 15;13(2):e0192360. doi: 10.1371/journal.pone.0192360. PMID: 29447188; PMCID: PMC5813927.


### Note :
Below is the codebase for the paper listed under reference.
https://www.cs.cornell.edu/courses/cs4780/2018fa/lectures/lecturenote17.html
