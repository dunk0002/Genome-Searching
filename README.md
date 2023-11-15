# NCBI Database Searching

This project was created to allow for automated searching of the National Center for Biotechnology Information (NCBI) database for genetic information on user desired species and genomes. The access number is then returned to make access easier. 

## Installing Necessary Packages

Install the necessary packages to access teh NCBI database and other aspects of project

``` python
pip install biopython
from Bio import Entrez
from Bio import SeqIO
from prettytable import PrettyTable
import pandas as pd
```

## Searching Database

One functions, `find_latest_genome`,find the latest genome from user input species and genome type from the NCBI database. It also allows for the output to be sent to the user's email that is input. The publication date, ideal reference sequence, and most recent match will be displayed to make searching less tedious in the database. 

The `get_reference_sequence` locates the reference sequence to the genome that the user asks to see.

Other features available are finding all the instances of the specific genome and outputting the data to an Excel file for easier access. 
