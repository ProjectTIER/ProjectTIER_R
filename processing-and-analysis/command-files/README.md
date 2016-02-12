# Command Files

This folder should contain one or more R scripts (with the `.R` 
extension) that contain commands that execute every step of data 
processing and analysis required to reproduce the results you report in 
your paper.

In all of the scripts you write, it is important to include comments 
that are detailed and clear enough to make it possible for someone not 
familiar with your project to understand the steps of data processing 
and analysis that are executed by the commands in the script.

For the purpose of constructing and organizing your scripts, you should 
think of the work on your project in terms of three phases, which we 
will call (1) importing, (2) processing, and (3) analysis. Your scripts 
will include one or more files that execute each of these phases of 
research.

1. For the importing phase, the script(s) should contain commands for R 
to read the data in each of your importable data files, and then save 
them in `.Rdata` format. For example, if you have an importable data 
file in `.csv` format, your script(s) will include a command like 
`read.csv()` that imports the data, and a `save()` command that saves 
the data in an `.Rdata`-formatted file. (If an importable data file is 
already in `.Rdata` format, nothing needs to be done to it during the 
importing phase.) <br><br> 
At the end of the importing phase, you will have a set of data files, 
all in R’s `.Rdata` format, containing all the data for your project. 
These data files will serve as inputs to the processing phase described 
below. <br><br>
When you have completed your paper, these files should not be included 
in the final documentation. Anyone interested in these files can create 
them simply by executing the R scripts you wrote for the importing 
phase of your project.

1. The script(s)for the processing phase should include commands that 
execute all the processing required to transform your importable data 
files into the final data file(s) that you will use in your analysis. 
Exactly what these steps will be is highly variable, but they typically 
include operations such as joining two or more data files, dropping 
variables or cases, generating new variables, and recoding. At the end 
of the script(s)for the processing phase, there should be `save()`
commands that save (in `.Rdata` format)the final data file(s) upon 
which your analysis will be conducted. We will refer to the final data 
files(s) that you use in your analysis as "your analysis data file(s)". <br><br>
If you have a single analysis data file - i.e, if all of your analysis 
will be performed using a single data file created during the 
processing phase - it should be saved with the name `analysis.Rdata`. 
If you have more than one analysis data file, give them informative 
names, such as `analysis_euro.Rdata`, `analysis_afri.Rdata`, and 
`analysis_asia.Rdata`; or `analysis_individual.Rdata` and 
`analysis_household.Rdata`. <br><br>
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