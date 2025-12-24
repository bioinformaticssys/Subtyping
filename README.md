#  CODE OF LRSFC
This is a Matlab separate executable program to identify cancer subtypes based on LRSFC: Subtyping Cancer based on Low-Rank
Representation and Similarity Fusion Clustering by Joint Multi-Omics Data. It provide a methodological framework for detecting disease subtypes.

MATLAB Compiler

1. Prerequisites for Deployment  <br>
. Verify the MATLAB Runtime is installed and ensure you have installed version 9.1 (R2016b).   
. If the MATLAB Runtime is not installed, do the following:<br>
   (1) enter <br>
      mcrinstaller<br>
      at MATLAB prompt. The MCRINSTALLER command displays the location of the MATLAB Runtime installer.<br>
   (2) run the MATLAB Runtime installer.<br>
Or download the Windows 64-bit version of the MATLAB Runtime for R2016b from the MathWorks Web site by navigating to

   http://www.mathworks.com/products/compiler/mcr/index.html
  
For more information about the MATLAB Runtime and the MATLAB Runtime installer, see  Package and Distribute in the MATLAB Compiler documentation in the MathWorks Documentation Center.    

NOTE: You will need administrator rights to run MCRInstaller. 

2. Files to Deploy and Package<br>
Files to package for Standalone <br>
================================<br>
-LRSFC.exe<br>
-MCRInstaller.exe <br>
   -if end users are unable to download the MATLAB Runtime using the above link, include it when building your component by clicking the "Runtime downloaded from web" link in the Deployment Tool
-This readme file <br>

3. Definitions<br>
For information on deployment terminology, go to http://www.mathworks.com/help. Select MATLAB Compiler > Getting Started > About Application Deployment > Deployment Product Terms in the MathWorks Documentation Center.<br>

## Instruction of LRSFC<br>

1. LRSFC.exe is a Matlab separate executable program for the routine of experimental analysis, implementing the LRSFC algorithm.

2. LRSFC is going to run by supplying following parameters: <br>

        (1)	input Folder: the directory locating of the omics data as the input data.
         Its default format is: each row represents features; the each column is a sample of data; the current form of data is : '.mat' . 
        (2)	output Folder: the directory locating of the cluster assignment as the output data. 
        (3)	parameter lambda: lambda values is set between  2^-15 and 2^15.      
        (4) number of clusters: required number of subtypes 

## Demo

*  Dependencies: Matlab R2016b <br>

* The LRSFC.exe is running as follows:  
LRSFC:C:\Users\SYS\Desktop\LRSFC\inputdata C:\Users\SYS\Desktop\LRSFC\outputdata 128 4


