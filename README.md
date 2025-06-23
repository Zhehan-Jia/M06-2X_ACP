# M06-2X_ACP
This repository provide the information of generating the corrected M06-2X/6-31+G(d,p) method using atom-centered potentials (ACPs) approach. 


# Targeted Improved Properties
1. Bond dissociation enthalpy (BDE)
2. Barrier height (BH)
3. Reaction energy (RE)
4. Non-covalent interactions (NCIs)


# Fitting data
The following benchmarks are used for as fitting data:
1. [BSE49](https://github.com/aoterodelaroza/bse49) ([prasad2021](https://www.nature.com/articles/s41597-021-01088-2.pdf).)
2. BH9 ([prasad2021](https://testpubschina.acs.org/doi/10.1021/acs.jctc.1c00694).)
3. BBI ([smith2016](https://pubs.acs.org/doi/10.1021/acs.jpclett.6b00780),[burns2017](https://pubs.aip.org/aip/jcp/article/147/16/161727/77022/The-BioFragment-Database-BFDb-An-open-data))
4. S66x10 ([rezac2011](https://pubs.acs.org/doi/10.1021/ct2002946).)

Their Cartesian coordiantes are also provided in [XYZ]()

# ACP terms
The 'ACP terms' are referred when calculating the electronic energies of the fitting data through non-self-consistent filed calculation under certain conditions. This current ACP terms are calculated when n = 2, *l*<sub>max</sub> = *d* (*l*<sub>max</sub> = *p* for Hydrogen), with 29 exponents (ζ) ranging from 0.12 to 3.0 at 0.001 coefficient. 

The example of term's input file can be find [Terms/Input_File]() and their energy contributions can also be found in [Terms/Energy](). The ACP terms were fit using [*acpdb* program](https://github.com/aoterodelaroza/acpdb).

# ACPs
The optimized ACPs is provided in [ACP](), and the example of using ACPs is listing in the same folder.
