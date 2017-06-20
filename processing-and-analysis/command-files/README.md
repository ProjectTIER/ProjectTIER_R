# Command Files

For simple implementations of the TIER Protocol, the "commands" (R code) will be interwoven with text in the `.Rmd` file in the main folder of your project. 

However, occasionally it is necessary to split out supplementary work into additional files. For example, you may have a separate `.Rmd` file that completes a long and arduous data cleaning process, or you may have R scripts (with the `.R` extension) that contain specialized functions you wish to "source" into your final analysis. 

These additional files should be placed in the `command-files` directory. 

In all of the scripts you write, it is important to include comments 
that are detailed and clear enough to make it possible for someone not 
familiar with your project to understand the steps of data processing 
and analysis that are executed by the commands in the script.

For the purpose of constructing and organizing your scripts, you may want to
think of the work on your project in terms of two phases, 
(1) processing, and (2) analysis. Your scripts 
will include one or more files that execute each of these phases of 
research.

1. The script(s)for the processing phase should include commands that 
execute all the processing required to transform your importable data 
files into the final data you will use in your analysis. 
Exactly what these steps will be is highly variable, but they typically 
include operations such as joining two or more data files, dropping 
variables or cases, generating new variables, and recoding. At the end 
of the script(s)for the processing phase, there should be `save()`
commands that save the final data file(s) upon 
which your analysis will be conducted. We will refer to the final data 
files(s) that you use in your analysis as "your analysis data file(s)". <br><br>
Your analysis data file(s) should be stored in your `analysis-data` 
folder. <br><br>
Strictly speaking, including your analysis data file(s) in the 
documentation is redundant:  anyone interested in your analysis data 
file(s) files can create them simply by executing the R scripts you 
wrote for the importing and processing phases of your project. 
Nonetheless, the TIER Protocol calls for your analysis data file(s) to 
be included simply because it is sometimes convenient to have a readily 
accessible copy of the analysis data.

1. The script(s) for the analysis phase should contain commands that 
open the analysis data file(s) you created in the processing phase, and 
then generate the results reported in your paper. <br><br>
Every command in your analysis script(s)that generates a piece of 
output or a result reported in your paper should be preceded by a 
comment that indicates what piece of output or result the command will 
generate.The following examples illustrate some typical kinds of 
comments:

    `# The following command produces Table 6.`

    `# The following command produces Figure 12.`
    
    `# The following command calculates the correlation of -0.54` <br>
    `# between variables X and Y reported on page 16 of the paper.`

All of the scripts for importing, processing and analyzing your data 
should be included in the `command-files` folder. 

One additional script, called `data_appendix.R`, should also be 
included in your `command-files` folder. This script is described in 
the instructions for your Data Appendix.