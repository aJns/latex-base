###################################################
# Simple Makefile for LaTeX-Documents             #
#                                                 #
# Erno Salminen, Decemeber 2012                   #
###################################################


#############################
##### Variables #############

# Basename for the document (without postfix '.tex')
TARGET=kandityo



#############################
##### Targets ###############
# Not all people use bibtex
all: ${TARGET}.tex
	rubber --force --pdf -I ../kuvat ${TARGET}.tex


rubber: ${TARGET}.tex
	rubber --pdf ${TARGET}.tex



# Clean. Remove generated files (aux=cross-references, dvi=device
# independent (kind of pdf clone), log=messages and errors, toc=table
# of contents, lof=list of figures...)
clean:
	rubber --clean ${TARGET}.tex
