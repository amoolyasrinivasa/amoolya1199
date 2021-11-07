# my_io.py
This is a python module that contains one function get_fh() which is used in all the three programs below. Anytime a file needs to be opened for reading or writing in your programs in this assignment, the program calls on this module's function get_fh() function. It can be imported using:
  from assignment4 import my_io or  from assignment4.my_io import get_fh
The module's get_fh() function can be called by: 
  fh_in = my_io.get_fh(infile1, "r")

# chr21_gene_names.py
This python program takes in the input file containing genes of human chromosome 21. For each gene, the file gives the gene symbol, description and category. The fields are separated by tabs. The program asks the user to enter a gene symbol and then prints the description for that gene based on data from the chr21_genes.txt file. The program gives an error message if the entered symbol is not found in the table.
## Description
The chr21_genes.txt file lists genes from human chromosome 21, in their order along the chromosome. 
The function get_description_dictionary(fh_in) Takes in the input file, reads it and returns a dictionary of descriptions corresponding to each category. 
## Getting started

## Dependencies
Runs on linux or any other CLI

## Installing
The programs can be found on the programming6200/assignment4 directory on defiance

## Executing programs
python3 chr21_gene_names.py -h
python3 chr21_gene_names.py -i chr21_genes.txt

# categories.py
This program counts how many genes are in each category based on data from the chr21_genes.txt file. The program prints the results so that categories are arranged in ascending order to an output file to the output file OUTPUT/categories.txt 

## Description
The chr21_genes.txt file lists genes from human chromosome 21, in their order along the chromosome and the HUGO_genes.txt file lists all human genes having official symbol approved by the HUGO gene nomenclature committee.
The function get_description_dictionary(fh_in) Takes in the input file, reads it and returns a dictionary of descriptions corresponding to each category. 

## Getting started

## Dependencies
Runs on linux or any other CLI


## Installing
The programs can be found on the programming6200/assignment4 directory on defiance

## Executing programs
$ python3 categories.py -h
$ python3 categories.py -i1 chr21_genes.txt -i2 chr21_genes_categories.txt

# intersection.py
This program finds all gene symbols that appear both in the chr21_genes.txt file and in the HUGO_genes.txt file. These gene symbols are printed to a file in alphabetical order into output file OUTPUT/intersection_output.txt. The program also prints on the terminal how many common gene symbols were found. 

## Description
The file chr21_genes_categories.txt is a file that contains the categories and the meaning of each category.

## Getting started

## Dependencies
Runs on linux or any other CLI

## Installing
The programs can be found on the programming6200/assignment4 directory on defiance

## Executing programs
$ python3 intersection.py -h
$ python3 intersection.py -i1 chr21_genes.txt







