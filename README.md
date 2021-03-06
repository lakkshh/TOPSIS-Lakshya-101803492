# Implementation of TOPSIS by Lakshya Gupta
This package calculates topsis/performance score for given .csv file, thus helping in Multiple Critera Decision Making (MCDM).

## Important Details

##### Input File

- The input file must be a .csv or .txt file only.
- The input file must have atleast three columns.
- The first column of the input file is the object/variable name. (e.g. X1, X2, X3, X4...)
- All columns except the first (name) column contain numeric values only.

##### Output File
- The output file contains two new columns i.e. Topsis Score and Rank along with the original columns.

##### Parameters for the **topsis** function are as follows
- The **input file name**. It must end with .csv or .txt. The complete file path must be given to read the file residing in a different directory.

- The **weights** string that contains the weights for each column separated by commas.
   Example: "0.25,0.25,0.25,0.25"

- The **impacts** string that contains the impacts for each column separated by commas.
   Example: "+,+,-,+"

- The **output file name**. It must end with .csv or .txt. The complete file path must be given to save the file in a different directory.

##### The **topsis** function must be called with all 4 parameters otherwise exceptions will be raised.

## 
## 
##

## Sample Use Case

```
import TOPSIS_Lakshya_101803492 as t
t.topsis("inputFileName.csv", "0.25,0.25,0.25,0.25", "+,+,-,+", "outputFileName.csv")
```
## 
## 

## Change Log

##### 0.0.65 (12/11/2020)
- First Release