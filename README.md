#MPKin-Simu
This is a software program to simulate pedigrees. This software was developed as part of MPKin [1] many years ago, and were also used in many other studies [2-5]. Because multiple requests were received for this particular software program, I decide to share this tool so that you may use as you wish. This software assumes all loci in simulation are independent, but allows mutation and population substructure. Only autosomal loci are used in the simulation. 

This software was written by JAVA, so it may be run on any platform that has the latest version of JAVA installed. 

##A quick start
The software may be run with the following commend

	java -jar MPKin-simu.jar NumOfReplicates Fst paf_file ped_file output_file

NumOfReplicates: the number of pedigrees you would like to simulate

Fst: population substructure correction

paf_file: a file contains the allele frequencies of a population and the mutation rates (both paternal and maternal) of the markers. See examples in the folder of AlleleFreq

ped_file: a pedigree file, which follows the same format as GATK Pedigree format, except that the last column was named as ¡°Pop¡± (i.e., population) but was not in simulation. See examples in the folder of CommonRelationships

output_file: the simulated pedigrees

For example:  

    java -jar MPKin-simu.jar 100 0.01 caucasian.paf fullsib.ped simupeds.txt


##How to cite:
Ge J, Budowle B, Chakraborty R. DNA identification by pedigree likelihood ratio accommodating population substructure and mutations. Investigative Genetics. 2010 Dec;1(1):1-9.

##Contact: 
For any questions or bugs, please contact  gejianye@gmail.com or Jianye.ge@unthsc.edu 
##References:
1.	Ge J, Budowle B, Chakraborty R. DNA identification by pedigree likelihood ratio accommodating population substructure and mutations. Investigative Genetics. 2010 Dec;1(1):1-9.
2.	Ge J, Budowle B, Chakraborty R. Choosing relatives for DNA identification of missing persons. Journal of forensic sciences. 2011 Jan;56:S23-8.
3.	Ge J, Chakraborty R, Eisenberg A, Budowle B. Comparisons of familial DNA database searching strategies. Journal of forensic sciences. 2011 Nov;56(6):1448-56.
4.	Ge J, Budowle B. Kinship index variations among populations and thresholds for familial searching. PLoS One. 2012 May 16;7(5):e37474.
5.	Ge J, Budowle B. How many familial relationship testing results could be wrong?. PLoS genetics. 2020 Aug 13;16(8):e1008929.
