# The TIER Documentation Protocol v2.0 for R

## Overview 

The TIER Documentation Protocol provides instructions for assembling a 
set of electronic files that document all the steps of data processing 
and analysis you conduct for an empirical research paper. 

The documentation specified by the Protocol contains all the data, 
computer programs, and explanatory information an independent researcher 
would need to be able to replicate the data processing and analysis you 
conducted for the project and to reproduce exactly all the results 
reported in your paper.

The instructions presented here are written for users of R.In a few 
places, they use R-specific terminology. For example, we refer to 
command files as scripts, and their names are followed by the .R 
extension. But the R-specific terminology that appears in these 
instructions can be easily translated to any of the major statistical 
packages (such as SPSS, SAS, Stata, Matlab, etc.) or other programming 
languages.

## Getting started

To get started you can fork or clone this repository which will create a copy of the folder structure recommended in the Project TIER protocol. Each folder comes with a README that describes what components of your analysis should go in that folder.

## Hierarchy of files and folders

Your repository should have the following hierarchy of files and folders:

- An electronic copy of your complete final paper
- The `README.md` file for your repository
- Original Data and Metadata - `original-data-and-metadata`
    + Metadata - `metadata`
        - Metadata Guide - `metadata_guide.md`
        - Supplements - `supplements`
    + Original Data - `original-data`
- Processing and Analysis - `processing-and-analysis`
    + Analysis Data - `analysis-data`
    + Command Files - `command-files`
    + Importable Data - `importable-data`

### Original Data and Metadata

#### Original Data

We use the term "original data file" to refer to a file from which you took any of the statistical data you used for your project.

Your `original-data` folder should contain a copies of all your original data files.

Any data that were necessary for any part of the processing and/or analysis you reported in your paper should be contained in one of the original data files in your `original-data` folder.

Every original data file should be saved in exactly the format it was in when you first obtained it.You may choose to change the name of an original data file when you save it in your `original-data` folder, but other than that the file should not be modified in any way.

#### Metadata

The top level of your `metadata` folder should contain one document: the Metadata Guide.

The `metadata` folder should also contain one sub-folder: the `supplements` folder.

The **Metadata Guide** is a document that provides information about each of your original data files. For every file in your `original-data` folder, the information in the Metadata Guide should include:

1. A bibliographic citation of the original data file in whatever editorial style (e.g., APA or Chicago) you have chosen to follow throughout your paper.
1. The date you downloaded, or obtained in some other way, the original data file.
1. Any unique identifiers, such as a Digital Object Identifier (DOI) or Universal Numeric Fingerprint (UNF), that have been assigned to the original data file.
1. A verbal explanation of how an interested reader can obtain a copy of the original data file.In many cases, this explanation will give the URL of a website from which the data can be accessed, along with instructions for downloading a file identical to the original data file you obtained from that site.In all cases, this explanation should be complete and precise enough to allow an independent researcher to locate and obtain the data file without any additional information or assistance.
1. Whatever additional information an independent researcher would need to understand and use the data in the original data file.The particular information required can vary a great deal depending on the nature of the original data file in question, and deciding what additional information to provide therefore requires thoughtful consideration and judgment.In many cases, the relevant information is similar to what is found in a codebook or users' guide for a dataset: variable names and definitions, coding schemes and units of measurement, and details of the sampling method and weight variables.In some cases, it is also necessary to include information about the file structure (e.g., the delimiters used to separate variables, or, in rectangular files without delimiters, the columns in which the variables are stored).Any other unique or idiosyncratic aspects of the data that an independent user of the data would need to understand should be explained as well.

If you used data from more than one original data file, the Metadata Guide should be comprised of multiple sections, with one section providing this information for each of your original data files.

The information specified in items (i)-(iv) should be presented in text that you write yourself.

The additional information described in (v) may also be presented in text that you write yourself.In some cases, however, some or all of the relevant additional information can be found in existing supplementary documents, such as users’ guides and codebooks that accompany the original data file. When relevant additional information is available in supplementary documents, it is not necessary to include this information in the text of theMetadata Guide. Instead, you may simply include copies of the documents that contain the relevant information in the documentation of your paper.These supplementary documents should be stored in the `supplements` folder.

For every document you include in the `supplements` folder, there should be comments in the Metadata Guide that
1. identify the document.
1. cite the source from which it was obtained.
1. indicate which of your original data files it pertains to.
1. state what relevant information it contains.

We composing the Metadata Guide as a Markdown document so that it can be rendered properly on GitHub, and any changes can be tracked. It should be named metadata_guide.md