# Mapping Multidimensional Poverty Indicator with Facebook Data

This repository is the product of my Masters Thesis. The code contained in here can be used to extend my analysis in other countries or augment it in other ways. 

In order to make this work a few additonal things are to do. 

1. Clone the repository PySocialWatcher from Joao Palotti and put the folder into the folder "Code". (And read their documentation of how to access the Facebook Marketing API to be able to actually collect Facebook data. Api key etc.)
2. Download the raw data necessary for this work. 


What to download?
First of all, all downloaded files should be put in a folder called "Raw Data" (several subfolders should be made for this to not get lost in all the data). 

1. DHS data. DHS surveys are the ground truth used for this work. All can be downloaded form the DHS website [here](https://dhsprogram.com/). Download all stata files for whichever country you are interested in (+geolocations, that is an extra files which needs to be requested)
2. DHS processing code. You can do this on your own, but to save you some time, the Oxford Poverty & Human Development Initiative has published some do-files useful to compute all you need for the MPI (multdimensional poverty index). To be found [here](https://ophi.org.uk/multidimensional-poverty-index/data-tables-do-files/). 
3. WHO guidelines for stunting and wasting. These are necessary (and maybe also need to be edited) to process the DHS data into a poverty index. To be found [here](https://www.who.int/tools/child-growth-standards/software) (this can be annoying to download, feel free to reach out to me if you have trouble [j.s.karl@lse.ac.uk](j.s.karl@lse.ac.uk)
4. World pop Data. These are population estimates on a granular scale. Easy to download on their website [here](https://www.worldpop.org/).

Afterwards, I recommend setting up a folder "Data Exports" to store, surprise, exported data. This should include some subfolders to organise files.

After all is downloaded and the data from Facebook is queries (this will take time), you can run the file Data_Cleaning.Rmd (this will need some editing depending on which variables you query) and Data_Analysis.Rmd (this might need some editing of the directories but should run smoothly otherwise). Feel free to edit this file to suit your needs. Don't forget to cite me. 

