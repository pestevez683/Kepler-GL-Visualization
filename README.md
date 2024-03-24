# Project Kepler

This project utilizes Kepler.gl for geospatial data visualization in Jupyter Notebook. Below you'll find useful information for setting up and working with Kepler.gl in your environment.

## Contribution guidelines

Issues and Suggestions: If you find a bug or have an idea for improvement, you can open an issue on GitHub. Please provide clear details, and if possible, include examples or screenshots.

Pull Requests (PR): If you'd like to contribute code, you can submit a pull request. Here's how:
1. Fork the repository.
2. Make your changes in a new branch.
3. Submit the pull request to the main branch of the repository.

Feedback and Comments:If you have any comments about the script or suggestions on how to improve the contribution process, feel free to share them in the issues.

## User Guide

The user manual of Kepler GL can be found at the following link: [Kepler.gl User Guide for Jupyter](link_to_guide).

## Key Errors

### Error Loading Models:

You may encounter errors while loading Kepler.gl models, such as: `Model class 'KeplerGlModal' from module 'keplergl-jupyter' is loaded but can not be instantiated.` On Windows systems, some versions of libraries may pose problems. The following versions were found to be compatible and allowed working with Kepler.gl:

- Jupyter Notebook 6.5.5
- pywidgets: 7.8.0
- node: 18.19.1
- widgetsnbextension 3.6.5

### Install Node.js

If you haven't installed Node.js yet, you can download and install it from the [official Node.js website](https://nodejs.org/).

### Steps to Change Jupyter Notebook Versions of pywidgets, widgetsnbextension

Check your current environment by running the following code in a Jupyter Notebook cell:
```python
import sys
sys.executable
```

Activate the environment by using the following command in Anaconda Prompt:
```
conda activate my_environment
```
Or, if you're working from the Windows terminal, add the Anaconda directory to the system PATH following the steps mentioned below.

Commands to Install and Verify Versions:
Use the following commands to install and verify the versions of widgetsnbextension and ipywidgets:
```
pip uninstall widgetsnbextension
pip install widgetsnbextension==3.6.5
pip show widgetsnbextension
```

Enable widgetsnbextension by running the following command:
```
jupyter nbextension enable --py widgetsnbextension
```
## Anaconda Directory to PATH
When installing Anaconda on your system, select the option to add its bin directory to the system PATH, or

Once installed on your PC:
1. Open the Environment Variables menu > Advanced > Environment Variables.
2. In the System Variables section, find the variable named Path > Edit > New.
3. Add the path to the Anaconda Scripts directory (C:\Users\YourUser\Anaconda3\Scripts)> Ok.
