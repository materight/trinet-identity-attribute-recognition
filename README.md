# A Multi-Task Learning Approach to Attribute Recognition and Re-Identification

A multi-task learning approach to person attribute recognition and re-identification. Written in PTorch, trained and evaluated on the Market-1501 dataset.

## Get started
This project was developed using Google Colab, to execute it:
- Create a `Deep Learning` folder in the Google Drive root. Alternatively, change the `GDRIVE_HOME_PATH` constant in the notebook to use a custom root path.
- Upload the `.ipynb` notebook to Google Drive.
- Upload the `dataset.zip` file to Google Drive into `Deep Learning/dataset/dataset.zip`. Alternatively, change the `GDRIVE_DATASET_PATH` constant in the notebook to use a custom dataset path.
- Run the notebook.

**Note:** different hyper-parameter combinations can be tested by changing the parameter values of the function `main`, called in the "Run" section. 

## Code structure
The notebook is organized in different sections:
- **Imports:** external libraries imports.
- **Dataset:** definition of the Dataset and BatchSampler classes and a utility to load and transform the data. 
- **Model definition:** implementation of the three models, each with its separate class.
- **Loss functions:** definition of the loss classes: ReIDLoss, AttributeRecognitionLoss and MultiTaskLoss.
- **Accuracy functions:** implementation of the accuracy functions used to evaluate the results for attribute recognition and re-identification.
- **Train and test:** the main logic for training and validating the models.
- **Run:** instantiation of dataset, model, optimizer and loss functions. The hyper-parameters can be configured here. 
- **Final predictions:** construct the final results for the test and query sets.
