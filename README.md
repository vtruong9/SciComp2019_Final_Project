Vi Truong 
Scientific Computing 2019 
Final Project 

This code is for looking at nucleosome patterns around similar places in the genome.
Specifically, it takes aligned nucleosome footprinting, a motif of interest, and a number of base pairs around your motif you'd like to examine (+/-). It finds all locations of that motif of interest in the S. cerevisiae genome, takes the nucleosome read count at those locations from the input file, and clusters them. This is output as a dataframe with as many rows as there were hits of your motif, and twice as many columns as you've specified in your input. 

It is built to run on a supercomputer via ssh. The input should look like this:
python demo.py yeast_strain_Norm.sgr motif_of_interest 500
in order to align all nucleosome footprinting data from yeast_starin_Norm.sgr +/-500bp from all locations of motif_of_interest.
