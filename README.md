# CD-hit
Temporary guide to for CD-hit in the lab. Will be migrated to [Daugherty Lab wiki](https://github.com/daugherty-lab/daugherty-lab.github.io/wiki) after completion.

Takes input (-i argument, fasta or fasta.gz format, required) and creates an output (-o argument) based on user-defined options. 

# Relevant arguments
*   c = cutoff (0.8 = 80% sequence identity)
*   T = processors
*   Several other parameters, like size cutoffs (-s, -aL, -aS), etc, can be added in. Type "cd-hit" or see `cd-hit-manual.txt` in this repo to see explanation of these.

# Installation
1.  Install conda (lightweight [miniconda](https://docs.conda.io/en/latest/miniconda.html) or bulkier [anaconda](https://www.anaconda.com/products/distribution))
2.  Create conda environment
    ```conda create -n cd-hit```
3.  Activate environment
    ```conda activate cd-hit```
4.  Install CD-hit
    ```conda install -y -c bioconda cd-hit```

# Usage
Input Note: If you're on macOS, you can drag your input file into your terminal window to autofill the path to your file
Output Note: no need for suffixes

*   Example #1:

    ```cd-hit -i /path/to/file.fa -o /path/to/output```

*   Example #2:

    ```cd-hit -d 0 -g 1 -i path/filename.in -o path/filename.out -c 0.8 -T 4```

# Troubleshooting
1. If you use a gapped fasta alignment, you'll encounter: "Discarding invalid sequence or sequence without identifier and description!". This can be solved by removing `-` from your sequences.

# Resources
1.  [CD-hit Wiki list of tools](https://github.com/weizhongli/cdhit/wiki)
2.  [CD-hit GitHub repo](https://github.com/weizhongli/cdhit)
3.  [CD-hit webserver](http://weizhong-lab.ucsd.edu/cd-hit)