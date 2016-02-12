# Analysis Data

This folder should contain:

- Your analysis data file(s) as described in the instructions for your `
command-files` folder.
- Your Data Appendix, `data_appendix.Rmd`.

## The Data Appendix

Your Data Appendix is a document that serves as a codebook for your 
analysis data file(s).

If the data processing phase of your research generated just one 
analysis data file, and all the results presented in your paper were 
derived from that single analysis data file, the Data Appendix should 
begin with a brief description of the analysis data file.

Typically, this description will say something about the scope of the 
sample or population the data represent, specify the unit of analysis, 
and indicate the number of observations. As in the case of the metadata 
that accompanies your original data files, however, exactly what 
information is relevant will depend on the nature of the analysis data 
file, so deciding which aspects you will describe in the Data Appendix 
will require judgment.

After the brief description of the analysis data file, the Data 
Appendix should present information about every variable in the 
analysis data file.The information presented about each variable should 
include:

- a complete definition of the variable (including coding and/or units 
of measurement).
- the name of the original data file(s) from which the variable was 
extracted or from which the variables used to construct it were 
extracted.
- the number of valid observations for the variable, and the number of 
cases with missing values.

For categorical variables, the information should also include:
- a frequency table.
- a bar chart showing the proportion of observations in each of the 
possible categories.

For quantitative variables, the information should also include:
- basic summary statistics: the mean, standard deviation, minimum, 25th 
percentile, median, 75th percentile, and maximum.
- a histogram.

If the results presented in your paper were derived from more than one 
analysis data file, the Data Appendix should include all of the above 
information - the brief description of the data file and the 
information about each of the variables contained in the file - for 
each of the analysis data files that was used.

The Data Appendix should be an R Markdown document so that it can be 
rendered properly on GitHub, and any changes can be tracked. It should 
be named `data_appendix.Rmd`. This file should be stored in the 
`analysis-data` folder.

This file contains plain text as well as R code that generates the 
summary statistics and figures described above.