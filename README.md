# README - Programming for Data Analytics final project

This is the GitHub repository for the final project for the Programming for Data Analytics module.  
****  

| Topic | Details |
|---------|-------------|
| **Module:**  | 4369 - Programming for Data Analytics  |
| **Lecturer:**  | Andrew Beatty  | 
| **Course:**  | Higher Diploma in Science in Computing (Data Analytics)  |
| **Year/Semester:**  | Year 1 / Semester 2  |
| **Student Name:**  | David O'Connell  |
| **Student ID:**  | G00438912  |
| **Student Email:**  | G00438912@atu.ie  |  

## Purpose of this Repository  
This repository contains the files and folders associated with the Programming for Data Analytics final project, the subject of which is a Jupyter Notebook demonstrating analysis of a data set. The data sets chosen for analysis are windspeed records from a selection of weather stations around Ireland.  
  
### Link to Repository
[PFDA Project](https://github.com/dvdgeroconnell/PFDA-project.git).  
  
### Raw Data Source
[Historical Data - Met Éireann - The Irish Meteorological Service](https://www.met.ie/climate/available-data/historical-data).

## About this README  
This README contains an overview of the purpose, contents and instructions for use of the *PFDA-assignments* repository.  
  
It has been based on the guidelines in [GitHub's documentation on READMEs](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes).  
  
More information on writing in Markdown can be found in [Github's documentation](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax). 
  
## Repository Structure and Contents  
This repository contains the following files and folders:  
  
### .gitignore  
A GitHub-generated template which may be customized with extra files (names or types) and folders that GitHub should exclude from the repository.  
  
### requirements.txt  
A list of packages from the Python install in the source environment required for the Jupyter notebook, script or program to run. The following command will install the packages in *requirements.txt*:  
```  
pip install -r requirements.txt
```  
  
### weather.ipynb  
A Jupyter notebook containing the project submission - an analysis of wind data for a selected set of weather stations downloaded from [Met Éireann](https://www.met.ie/climate/available-data/historical-data).  
[Jupyter Notebook](https://jupyter.org/) is a web-based interactive environment used to create notebook documents that can contain live code, equations, visualizations, media and other computational outputs. Jupyter notebooks are often used by programmers and data scientists to document, experiment, document and demonstrate code-based workflows.  
  
### wind2.db
This is the [sqlite](https://www.sqlite.org/) database which contains the consolidated, cleaned and normalised wind speed data for the selected weather stations. It may or may not be present in the repository - if it is not,  it will be created by the notebook when it is run and will be used thereafter.

### subdirectories
The following subdirectories are included.  
  
#### ./data
Contains the files with the hourly, daily and monthly csv-formatted data, downloaded from Met Éireann for the selected weather stations. It also contains the files which explain the fields in the csv files, and a file called *poweroutput.txt*, which contains data on the performance of the [Siemens SWT-3.0-101 3MW wind turbine](https://www.thewindpower.net/turbine_en_275_siemens_swt-3.0-101.php).  
  
#### ./img  
Contains the image files used in the *weather.ipynb* notebook.  
  
## Getting Started  
To use this repository, the following steps apply:  
1. Clone this repository, either  
  a) to your local machine - [Visual Studio Code](https://code.visualstudio.com/download) and [Anaconda](https://www.anaconda.com/download) are pre-requisites.  
  b) using [GitHub Codespaces](https://github.com/features/codespaces) - click the green `Code` button at the top of the repository and select Codespaces.  
2. Review the README (this document).  
3. Open the *weather.ipynb* notebook in Visual Studio Code.  

## Running and Testing the Notebook
No special steps are required, once the pre-requisites are in place.  
  
Behaviour with and without the database may be tested. If the database is not present, it is built when the notebook is run and used each time the notebook is run, until such time as it is deleted again. To test behaviour without the database present, simply delete *wind2.db* from the repository.

## References

The [Programming for Data Analytics](https://vlegalwaymayo.atu.ie/course/view.php?id=10462) lectures were heavily referred to for this project.  

See the ***About this Readme*** section above for information on the resources used to write this document.
  
See the ***References*** section in the *weather.ipynb* notebook for the references used to develop the project. 
