Binding site search 

This program defines and applies functions to search the sequence elements for the presence (and number of occurrences) of the Sox consensus site and a Pax3 binding site. 

To be able to run this code, the following libraries should be installed with this code:

```
from Bio.Seq import Seq
from Bio.SeqRecord import SeqRecord
from Bio import SeqIO
import urllib
import seaborn as sns
import pandas as pd
```

The code is presented in a notebook and annotated with markdown to make it easy to use and understand. A brief overview of the code is:

1. Takes the sequences of the potential Sox10 enhancers and writes them to FASTA files with SeqIO. 
2. Defines functions to search for all variations of the Sox and Pax3 binding site sequences in the enhancer sequences, and print the number of times they occur and their position. 
3. Visualises the output in a bar chart.

Although I have used the function on my zebrafish sequence data, you could use it to search through any FASTA file you had. 
