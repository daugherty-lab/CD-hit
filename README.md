# CD-hit
CD-hit setup for the lab

Takes input (-i argument, fasta or fasta.gz format, required) and creates an output (-o argument) based on user-defined options. See file `cd-hit-manual.txt` or use `cd-hit` at the command line to prompt a comprehensive list of options.

# Installation
1.  Install conda (lightweight [miniconda](https://docs.conda.io/en/latest/miniconda.html) or bulkier [anaconda](https://www.anaconda.com/products/distribution))
2.  Create conda environment
    ```conda create -n cd-hit```
3.  Activate environment
    ```conda activate cd-hit```
4.  Install CD-hit
    ```conda install -c bioconda cd-hit```

# Relevant arguments
TBD

# Resources
1.  [CD-hit Wiki list of tools](https://github.com/weizhongli/cdhit/wiki)
2.  [CD-hit GitHub repo](https://github.com/weizhongli/cdhit)
3.  [CD-hit webserver](http://weizhong-lab.ucsd.edu/cd-hit)