# Indoor Air Quality Improvement with Filtration and UVC

## Purpose: 

This is to document our analysis and allow for a studying of the code and models used. All coding was done in either excel (minor things not included) or R; which produced most of the analysis and some of the graphics. 

## Where to Find Things:

There are currently two folders. One (CFU) is for bacterial data and it's analysis and the other (PM) is for particulate matter size data and it's analysis. Currently data is being withheld; interested parties are encouraged to contact the authors of the corresponding paper or the github repo owner for possible access. The files are saved as .Rmd files.

The analysis and corresponding code withen the CFU folder is fairly straight forward as a linear model. 

The code for the analysis of PM relies heavily on the package nlme for the gls() funciton to allow for fitting of general least squares. This is needed to account for the correlation structure inside the data (collected every five minutes for multiple days). The code for the plots of the models, using base R, is involved but one can follow it. The general layout is, sequentially, [1) Model fitting + anova, 2) CV model fitting, 3) Comparison] for all sizes of particulate matter studied. 
