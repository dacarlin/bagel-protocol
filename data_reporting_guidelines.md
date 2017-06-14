# Bagel Project Guide to Reporting Data

After you have completed production, purification, kinetic assay, and thermal denaturation assay on your batch of mutants, here's how to collect all the data into a report.

For each mutant, the following things should be included. Each item has a one-word name, a brief description including a unit of measurement (if necessary), and an example of use. Sometimes there is more than one example. 

# Data Descriptions & Formatting Rules 

## mutant_name

**Description**: The mutant name

**Format**: A string in the form `{native residue}{position}{designed residue}`, where `{native residue}` and `{designed residue}` are one-letter amino acid codes and `{position}` is the 1-indexed integer position of the residue in the BglB model sequence 

**Example**:

> E164A

## researcher

**Description**: Name of the undergraduate student researcher(s) who designed and characterized this mutant

**Format**: One or more names

**Example**: 

> Alex

> Amy, Ryan A., Ryan B.

## box

**Description**: The physical location of the plasmid encoding this mutant, box number.

**Format**: Integer 

**Example**:

> 2

## row

**Description**: The physical location of the plasmid encoding this mutant, row letter.

**Format**: A letter (A-Z) indicating a row in the box 

**Example**: 

> B

## column

**Description**: The physical location of the plasmid encoding this mutant, column number. (A lot of the boxes only have columns up to 9.)

**Format**: Integer indicating a column number 

**Example**: 

> 8

## expression

**Description**: An answer to the question: "Does the mutant appear on a gel after 2 independent attempts to produce and purify?" (Note: if the mutant does not express, only the next section (gel image) is relevant. For all other sections, the entry is "N/A".)

**Format**: `1` for yes, `0` for no

**Example**: 

> 0

## gel_number

**Description**: The index of the gel that this mutant appears on. Gels for a given data set are labeled in order from 1. Gel images should be saved on the gel imaging computer completely labeled. Ladder should be labeled with its name, e.g. "Thermo PAGE-Rule". Mutants should be labeled with their names. Wild type proteins should be labeled as "WT". It's not necessary to further distinguish wild type proteins.

**Format**: Numerical index

**Example**: 

> 4

## protein_yield

Protein yield as assessed by A280. If the protein does not express, do not report A280 (or any of the following functional parameters).

mg/mL

> 1.28

## kcat

The measured <em>k</em><sub>cat</sub> for this mutant, as determined by kinetic assay and fit using <a href="bagel.genomecenter.ucdavis.edu">bagel.genomecenter.ucdavis.edu</a>. The published limit of detection for our system is 1 min<sup>&minus;1</sup>. The maximum value for  <em>k</em><sub>cat</sub> we have observed so far is 1.1 &times; 10<sup>4</sup> min<sup>&minus;1</sup> (R240A), and the wild type BglB protein has a <em>k</em><sub>cat</sub> of 8.8 &times; 10<sup>3</sup> min<sup>&minus;1</sup> to an error of about 5%.

min<sup>&minus;1</sup>

> 1.44e3

> 834.23

> 3.4

## kcat_err

The measured standard error (one standard deviation error) of the fit to the Michaelis-Menten equation as determined by kinetic assay for the kcat parameter.

> 1.3e2

> 6.22

> 0.13

## km

The measured K<sub>M</sub> for this mutant as determined by kinetic assay (see "kcat" for more).

mM

> 5.52

> 0.21

> 15.50

## km_err

The measured standard error (one standard deviation error) of the fit to the Michaelis-Menten equation as determined by kinetic assay for the KM parameter.

> 0.43

## kcatkm

Measured kcat/km. ("<10" for mutants with activity below LOD, linear fit, or kcat/(1e-3*KM)

M<sup>&minus;1</sup>min<sup>&minus;1</sup>

> 1.74e5

> 918.3

> <10  

## kcatkm_err

Standard error (1 std. dev.) for the quotient kcat/KM. The standard error for ranges such as <10 should be reported as "NaN". [You may recall](http://www.fas.harvard.edu/~scphys/nsta/error_propagation.pdf) that for a quotient `Q=a/x`, the uncertainty `sigma(Q)` can be calculated as `abs(Q)*sqrt((sigma(a)/a)^2+(sigma(x)/x)^2))` when the standard errors `sigma(a)` and `sigma(x)` are known.

M<sup>&minus;1</sup>min<sup>&minus;1</sup>

> 1.2e2

> 5591.2

## tm

Measured functional protein melting temperature T<sub>m</sub> as determined by thermal stability assay.

˚C

> 39.2

## tm_err

Standard error (1 std. dev.), Tm

C

> 3.1

## data_complete

Data for this mutant is complete. Is the data for this mutant 100% correct and complete?

`1` for yes and `0` for no (default: `0`)

> 1

# FAQ

## Why are all the names lowercased single words with underscores instead of spaces?

The names are formatted this way to make nicely-named header columns in a pandas DataFrame. 
