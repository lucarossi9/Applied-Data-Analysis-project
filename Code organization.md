```console

├── Code
├── Project 2.ipynb: It contains the main analysis which show the feasibility of the project.
├── speaker attributes analysis.ipynb: It contains an anaysis of the speaker_attributes file (missing values, correlations, ...).
├── README.md: It contains an abstract and the detailed ideas for the project.
├── Data_transformation_notebooks
│   ├── Map Dates: It is the file used to create the correspondence between each quote and the dates in which the quote appeared in different articles.
│   ├── Filter quotes: The file used to filter the quotes about a given politician from the quotes centric dataset Quotebank.
|   ├── Problems to report: A file containing an issue found when extracting information from the article centric dataset.
|   └── Tranform special attributes: The file used to replace the ids in the speaker attribute file.
|   
```

Order in which the files can be reproduced:
1) Run speaker attribute analysis ---> exploratory analysis
2) Run Filter quotes ----> to filter the quotes
3) Run Tranform special attributes ----> to replace ids in the speaker attributes file
4) Run Map Dates ----> To have the date for each quote 
5) Run Project 2 -----> To make analysis