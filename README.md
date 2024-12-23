# Process Capability Analysis
This project was design to allow me, and now others, to do statistical analysis of an industrial process in a fast and intuitive maner.
It was also designed to allow users with low or no proficiency in Python or Jupiter Notebooks to use it.
**It is important to note that it was designed to be used in Google Colab, otherwise some functions may have to be modified accordingly.**
The needed inputs are the excel spreadsheet with the data, the process variable column, the column to group (time,...) and specs.
First, I defined the different functions for the data analysis, and they are called into a final function called report.
In the report, first it tests if the distribution is **normal**, if not the methods used here may not apply.
Secondly, it calculates process capability indexes, such as **Cpk & Cp** (assuming normal distribution), and once again tells you what is the actual distribution of the system.
The third step is to test the process variable agains the **Nelson rules test** (also known as Western Electric Rules) and plot it in a process chart.
The last step is the use of **multivariant analysis** to check the impact of each process variable in the other ones. 
It's limited to the first 10 variables, but the code can be changed to include more or less.
The accepted input is an excel file.
Follow the instruction in the beginning of the code, the analysis is automated and the report will be automatically downloaded to your machine.
