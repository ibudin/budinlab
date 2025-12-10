## Setting up platform
Using Anaconda, launch Visual Studio Code, pycharm, Jupyter Notebooks etc. or any platform you are most comfortable with

Make sure the kernel you are using is the latest version of Python (this code runs with version 3.10)

If you do not have the packages installed, in the terminal (In pycharm you may have to install the packages for each individual project):
pip3 install numpy
pip3 install pandas
pip3 install seaborn
pip3 install matplotlib
pip3 install scikit-image
pip3 install nibabel

## Running the code
Copy and paste the code into you new window

Locate the file paths of the necessary files/directories on your device

Open the cell image on FIJI and determine the threshold value

In each of following codes, and example of calling the function is provided at the end, you must modify these with your own file paths and values

All file paths must be a string, i.e. ' /Users/yourname/Desktop/test.tif '
  
  allplotsGP
  
    Call the function (after the code):
    
    GpCalculationStack(gp_im_stack, cell_im_stack, thresh)
    
    gp_im_stack: file path of the standard images 
    
    cell_im_stack: file path of the cell image specific stack
    
    thresh: determined threshold value
    
    Outputs will be saved on your device, must search for final.tif and GPs.txt

  calcGP

    Call the function (after the code): 
    
    GpCalcIter(gp_im_stack, cell_im_dir, final_dir, thresh)
    
    gp_im_stack: file path of the standard images 
    
    cell_im_dir: directory of the cell image stacks
    
    final_dir: directory of the where you want the outputs to be saved
    
    thresh: determined threshold value  
    
    Outputs will be saved in specified folder
    
    Call the function (after the code): 


  GivenGpIter(gp_corrected, cell_im_dir, final_dir, thresh)
  
    gp_corrected: value (float) of the calculated GP correction value outputted from the standardvaluesGP script
    
    cell_im_dir: directory of the cell image stacks
    
    final_dir: directory of the where you want the outputs to be saved
    
    thresh: determined threshold value
    
    Outputs will be saved in specified folder

  standardvaluesGP
    
    Call the function (after the code): 
    
    StandardIter(standard_dir, standard_finish)
    
    gp_im_stack: file path of the standard images 
    
    standard_dir: directory of the standardl image stacks
    
    standard_finish: directory of the where you want the outputs to be saved
    
    Outputs will be saved in specified folder
