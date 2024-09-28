# Drug Resistance Prediction

## Project Goal

Antimalaria Resistance Prediction Machine learning project

## Project Desciption

---

### Interacting with the Project UI

On the UI, we have the option to upload a file from our computer or enter a link to _.fa_ file. We then proceed to the dropdown provided and select the drug we want to test for. The result is outputted and there is an option to download to a csv file.

## Links, Folders and Files

### Links

- Project Interface:
- GitHub Repository: https://github.com/profgreatwonder/resistance-prediction
- Documentation: https://github.com/profgreatwonder/resistance-prediction#README

### Folders and Files

- **archived**: contains unused notebooks
- **consensus_sequences**: contains the ".fa" files
- **csv_dataset_files**: contains the csv files representing the drugs used in training the models
- **datadict_files**: contains csv files generated during model training
- **model_training_notebooks_binary_classification_random_forest**: contains notebooks used in training the different models with the dataset representing the different drugs.
- **pickle_files**: contains pickle files used in prediction stored in app.py
- **xlxs_dataset_files**: contains excel files which were converted to csv files for training
- **app.py**: contains the logic responsible for the UI that gives access for the model to be used in prediction
- **README.md**: contains the project documentation
- **requirements.txt**: contains the technologies used and their versions. Used by streamlit to deploy the app on their servers. gotten by running the command below inside of our activated environment, saving it to a ".txt" file and editing:

        pip list

- **requirements.yml**: also contains technologies used and their versions. Used to recreate the project using conda on your local machine. This file is gotten from running the command:

        conda env export --no-builds > requirements.yml

**Note 1**: _--no-builds_ makes sure that the technologies are not generated with the versions specified to the operating system used for the project.

**Note 2**: the code below present in all the notebook is important to help generate the present working directory for your machine. With it, you can replace the filepath present in the project with the right location on your local.

        import os
        print("Current working directory:", os.getcwd())

## Dataset Description

## Software and Tools

1. VSCODE
2. Jupyter Notebook
3. Git/Github
4. Streamlit

## Replicating the Project

The environment was created, activated and requirements stored in yaml file by running the following commands:

for .yml

- conda create --name ML-Project-on-Resistance-Prediction
- conda activate ML-Project-on-Resistance-Prediction
- conda env export --no-builds > environment.yml

To replicate the environment, do the following:

- Clone the Project
- Create the environment and install all requirements by running the command:

      conda env create -f environment.yml

for .txt with conda

- conda create --name ML-Project-on-Resistance-Prediction
- conda activate ML-Project-on-Resistance-Prediction
- conda list --export > requirements.txt

To replicate the environment, do the following:

- Clone the Project
- Create the environment and install all requirements by running the command:

        conda create --name <env_name> --file requirements.txt

To run the streamlit UI, we have to run the command below in our terminal:

        streamlit run app.py

## Summary of Findings

## Conclusion
