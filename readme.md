
# Wrangling climate data 
## Aim of this talk was to show how to extract publically available climate data and use various open source python modules to wrangle multi-dimensional climate data. 


![alt text](https://github.com/jeev20/WrangleClimateData/blob/master/images/9.png "Wrangling_Climate_Data")
--------------------------------

## Installing dependencies

* Main dependency: Python 3.6 

* Clone the repo and follow the following steps 


### Basemap on Windows without anaconda
Using basemap on windows without anaconda is a complicated task. Using pip to install basemap requires some additional steps. 

I have tried to make it simple here by providing you the necessary steps needed to get this to work in windows. 

If you are using a linux enviornment and / or anaconda in windows these hurdles are next to non-existent! 
``` 
conda install basemap
```

Step 1

* If your are not using conda to install basemap, download the basemap module from this link: https://www.lfd.uci.edu/~gohlke/pythonlibs/#basemap 

IMPORTANT: Depending on the python version you have in your system download the appropriate amd64.whl version.

* Download this file and move it to the project folder (git cloned folder): "basemap‑1.2.2‑cp36‑cp36m‑win_amd64.whl"


Step 2
* Download the sample netcdf data from this link "https://drive.google.com/file/d/1posMq2_3pM5G-8fNneGJI96Ypa7Hs8Lc/view?usp=sharing"

* The talk covers different sources you can use to get such netcdf files, but the file about is just a sample required to run the juypter notebook

* Move the downloaded file to the "Data" folder in the project directory


Step 3 
* Open powershell in the project folder path
* Activate a virtual environment in the project folder in your virtual environment

If you dont have a virtual env set up 
a. Install virtualenv to your main python installation (global install)

``` 
pip install virtualenv  
```

b. Navigate to the cloned folder of the repo and run  (this creates a virtual enviornment)
``` 
virtualenv env  (You can name it as you like. Here I use "env")
```
c. Activate the virtual enviornment 
``` 
env/Scripts/activate   (For windows) 
```
d. Now you will see the "env" showup in the command line. This means you are on a virtual enviornment of python

Step 4

To install basemap in windows use (Ensure Step 3 is done else you will install these onto the global python installation)
``` 
pip install basemap-1.2.2-cp36-cp36m-win_amd64.whl 
```

This command should install all other project dependencies. requirements.txt contains the list of modules required.
```
pip install -r requirements.txt 
```

## Usage

Step 5
Run jupyter notebook from the project directory

```
jupyter notebook
```

Step 6
Double click on the file : "Wrangling_climatedata.ipynb"

## Contributors
* jeev20

