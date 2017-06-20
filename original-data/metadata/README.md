# Metadata

The top level of your `metadata` folder should contain one document: 
the Metadata Guide.

The `metadata` folder should also contain one sub-folder: the `
supplements` folder.

## Metadata Guide

For each of your original data files, the Metadata Guide provides the kind of information typically found in a codebook accompanying a dataset, such as variable definitions and coding, sampling methods, and anything else a user would need to know to work with and interpret the data appropriately.  

You, the author of the paper, compose the Metadata Guide.  

The Metadata Guide should be organized into one or more sections; each section should provide information about one of the original data files in your `original-data` folder.  For each original data file, the information included in the Metadata Guide should include:


1. *A bibliographic citation for the original data file.* This citation should be in a format consistent with the editorial style (e.g., APA or Chicago) used in the main paper or report on the study.
1. *A digital object identifier (DOI) for the data file (if one has been assigned).* If a DOI is included in the bibliographic citation, it need not be repeated.
1. *The date on which the author first downloaded, or obtained in some other way, the original data file.* If a date is included in the bibliographic citation, it need not be repeated.
1. *A written explanation of how an interested reader can obtain a copy 
of the original data file.* In many cases, this explanation will give the 
URL of a website from which the data can be accessed, along with 
instructions for downloading a file identical to the original data file 
you obtained from that site.In all cases, this explanation should be 
complete and precise enough to allow an independent researcher to 
locate and obtain the data file without any additional information or 
assistance.
1. *Whatever additional information an independent researcher would need 
to understand and use the data in the original data file.* The particular 
information required can vary a great deal depending on the nature of 
the original data file in question, and deciding what additional 
information to provide therefore requires thoughtful consideration and 
judgment.In many cases, the relevant information is similar to what is 
found in a codebook or users' guide for a dataset: variable names and 
definitions, coding schemes and units of measurement, and details of 
the sampling method and weight variables.In some cases, it is also 
necessary to include information about the file structure (e.g., the 
delimiters used to separate variables, or, in rectangular files without 
delimiters, the columns in which the variables are stored).Any other 
unique or idiosyncratic aspects of the data that an independent user of 
the data would need to understand should be explained as well.
1. *Supplementary documents with additional metadata.* In many cases, some or all of the information about an original data file that should be included in the Metadata Guide is available in an existing, publicly accessible document, such as a codebook or user’s guide that is provided with the original data file.  In these cases, it is not necessary to include that information in the Metadata Guide.  Instead, you may simply put a note in the Metadata Guide indicating that the information is available in an existing document.

When you put a note in the Metadata Guide indicating that certain parts of the information that should be provided there are available in an existing document, you should preserve a copy of the existing document in the Metadata sub-folder (along with the Metadata Guide that you compose yourself). 

The Metadata Guide should be a Markdown document so that it can be 
rendered properly on GitHub, and any changes can be tracked. It should 
be named `metadata_guide.md`. This file should be stored in the 
`metadata` folder.