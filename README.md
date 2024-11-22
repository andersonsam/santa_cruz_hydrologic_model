# Santa Cruz Hydrologic Model 
  
This repository contains Python code that computes plausible climate change hydrology for the city of Santa Cruz, CA.  The original MATLAB version was created by Dr. Shawn Chartrand.  The MATLAB version was translated into Python by Dr. Sam Anderson. 

___ 
## How to use 

### Set up Python environment  

#### Option 1: Create environment directly in terminal  
1. Create a new folder/directory called 'santa_cruz_hydrologic_model' in the desired location.
2. In terminal, navigate to santa_cruz_hydrologic_model.
3. Use conda to create a virtual environment by entering the following text in the terminal window:
   * conda create -n santa_cruz_hydrologic_model python=3.11 numpy=1.26.4 pandas=2.2.1 matplotlib=3.8.0 tqdm=4.66.2 jupyterlab=4.0.11
4. Activate the environment by entering the following text in the terminal window:
   * conda activate santa_cruz_hydrologic_model
5. Open Jupyter Lab to run the .ipynb files by entering the following text in the terminal window:
   * jupyter lab
  
#### Option 2: Create environment from .yml file in terminal
1. Create a new folder/directory called 'santa_cruz_hydrologic_model' in the desired location.
2. In terminal, navigate to santa_cruz_hydrologic_model.
3. Use conda to create a virtual environment by entering the following text in the terminal window:
   * conda env create -f environment.yml
4. Activate the environment by entering the following text in the terminal window:
   * conda activate santa_cruz_hydrologic_model
5. Open Jupyter Lab to run the .ipynb files by entering the following text in the terminal window:
   * jupyter lab  

### Set up directory structure  

* Python
  * Input
    * TBD
  * Input_Climate
    * TBD
  * Input_Historical
    * TBD
  * Output_HISTORICAL_SIM_Python
    * This is where the code will save all outputs.  The code will automatically create sub-folders here that are named the same as the scenario. 
  * Code files (.ipynb)
* MATLAB
  * Input
    * TBD
  * Input Climate
    * TBD
  * Input Historical
    * TBD
  * Output HISTORICAL SIM
  * Code files (.m)
* environment.yml   

### Run test code 

Test examples of code use are provided in the file 'example_use.ipynb'.  Run 'example_use.ipynb' to save results for the provided model scenarios.

### Compare test results with MATLAB results  

The Python results can be compared with results from the MATLAB version to ensure consistency. Run 'python_matlab_compare.ipynb' to visualize the similarity between all variables in both model versions.  All variables have been tested by SA and SC and found to be equivalent between the two model versions. 

___  
## Description of files  

example_use.ipynb  
  * This file is the main file to use for hydrology simulations

python_matlab_compare.ipynb  
  * This file is for testing to ensure that the Python version results are equivalent to the MATLAB version results

HCPHydroDFG5Base_Project2020_CC_AdultRev_UMass.ipynb  
  * This file contains the main function for computing hydrology simulations.  This function calls and uses the five following functions during its computation.

CC_DailyFlow_Historical_Northcoast.ipynb  
  *  TBD  

CC_DailyFlow_Historical_Rev.ipynb  
  * TBD  

CC_DailyFlow.ipynb    
  * TBD  

HydrologicCondition.ipynb  
  * TBD  

WaterBalance_MonthlyFlow.ipynb  
  * TBD  

___  
## Requirements  

python=3.11  
numpy=1.26.4  
pandas=2.2.1  
matplotlib=3.8.0  
tqdm=4.66.2  
jupyterlab=4.0.11  


