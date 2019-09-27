# Google Form Survey Analysis
This project is intended to help anyone analyze responses to a survey or other questionnaire conducted with Google Forms.

## Background
The code here was originally developed to help the volunteer [Bicycle & Pedestrian Committee](https://github.com/croton-on-hudson/bicycle-pedestrian-committee) of the village of Croton-on-Hudson analyze a survey of local residents.

## Code
The code is written in the [python](https://www.python.org/) programming language, using the [pandas](https://pandas.pydata.org/) data analysis library.  It is intended to be run as a [Jupyter Notebook](https://jupyter.org/).

## Setting up your environment
To run the code, we recommend installing [Anaconda](https://www.anaconda.com/distribution/), which includes everything you need.

Steps:
1. Fork this repository
2. Clone your fork onto your local machine
3. Download and install Anaconda  
4. Launch Anaconda Navigator and click the Jupyter Notebook icon therein
5. In Jupyter, open up the files in this repository

## Importing Google Form data
You must currently manually export your data from a Google Form survey or questionnaire.

1. Go to your Google Form survey
2. Click the `Responses` tab.
3. Click the spreadsheet icon towards the top right - this creates a Google Sheet with the responses in it
4. In that Google Sheet, click the `File`->`Download`->`Comma-separated values` menu option.
5. Save this file as `responses.csv` into your repository directory
6. If your survey responses could contain sensitive or private information, make sure your `.gitignore` file excludes this and other .csv files from version control - the example included here does so.

## Cleaning up the data
Run each of the notebooks one at a time in sequential order to clean up the data.  Each program contains specific instructions as a comment at the top of the code.
1. `cleanup.ipynb` - this program performs basic cleanup of the data
2. `free_text_tagging.ipynb` - this program asks you to manually assign tags to any free text response fields in your survey so we can organize and quantify them later based on those tags
3. `multiple_answer_cleanup.ipynb` - this program cleans up respones to survey questions with checkboxes that allow the respondent to select more than one answer option or to enter a custom 'other' free text response.

## Analyzing responses
4. `preliminary_analysis.ipynb` - this program analyzes multiple choice questions and outputs statistics and charts to show the results.
5. `multiple_answer_analysis.ipynb` - this program analyzes checkbox questions that allow more than one answer option or enter a custom 'other' respones, and outputs statistics and charts to show the results
6. `free_text_analysis.ipynb` - this program analyzes responses to any open-ended text fields on your survey and outputs statistics and charts to show the results as well as the text responses themselves.

## Contributing to this project
There is still work to be done to make this project easier to use and more powerful.

Check out our [contributor guidelines](CONTRIBUTING.md) if you'd like to get involved.

