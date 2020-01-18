# README
This repository contains all the code necessary to reproduce the analysis for the sample seminar project example for Susan Sayre's ECO 324 class at Smith College. It serves as a template for the material that should be included in a complete project. This README document provides an outline orienting the user to the material contained in the repository. 

*After reading this file, your audience should understand the structure of your project. As with the other documents in this sample repository, notes in italics (like this one) document their use and should be removed from your versions before submission.*

The template project is based on work completed by Simren Nagath ('19) for her seminar paper completed Spring 2019.

The root directory of the project contains the following files:

1. `MetadataGuide.Rmd` contains descriptions and documentation of the raw data files used in the project along with code for reading the files into R and dataframe summaries created using the `summarytools` package. *Depending on your project details you may or may not include code for merging different files together in your metadata guide. It is acceptable to include these steps in the metadata if they are relatively short and straightforward. Complex merge operations will appear in the next file. If merging is done in the Metadata Guide, that should be stated here.*

2. `DataConstruction.Rmd` contains a description of the steps along with the code used to transform the raw data files into the final variables used in the regression analysis. Each variable used in a regression is documented in the file, which also creates a table of variables and a table of summary statistics.

3. `FinalPaper.Rmd` produces the final paper. Code to run the regressions and create the output is embedded in the document.

These files create and/or draw on material stored in the following folders:

- `raw_data/` contains all the original, unaltered files used in the analysis. These files are documented in the Metadata Guide.
  
- `importable_data/` contains importable versions of the park visitation files whose creations is described in the Metadata Guide. *Delete this entry from this Rmd file if you did not need to create importable data files.*
   
- `processed_data/` contains intermediate datasets created during the project. *For this project, you should store your datasets that are created by the Metadata Guide and the Data Construction files in this folder, so that the code in each .Rmd document can run independently of the other files. In a typical research project, it would be more common to have the code in a separate .R file and source it in each document where it is needed. If you are familiar with this workflow and want to adapt these templates to use that, you are welcome to do so provided you check with me first.*

- `output/` (optional) contains other files created by the code. *This will generally be figures or tables that need to be used in multiple .Rmd files. Delete this entry and the corresponding folder if you do not have non-data output created by any of your .Rmd files.*
