# Bagel Team data reporting guidelines

After you have completed production, purification, kinetic assay, and thermal denaturation assay on your batch of mutants, collect all the data into a report. The following things should be included (some may recognize these as the columns from certain Google Docs, not sure whose idea that was originally (Trello?) but they should get credit for it) 

Each item has a one-word name, a brief description including a unit of measurement (if necessary), and an example of use. Sometimes there is more than one example.  

## mutant_name 

The mutant name 

> E164A

## researcher 

Name of the undergraduate student researcher who did the work. 

One or more names 

> Alex 

> Amy, Ryan A., Ryan B. 

## box

The physical location of the plasmid encoding this mutant, box number. 

Numerical index 

> 2 

## row

The physical location of the plasmid encoding this mutant, row letter. 

Alphanumerical index 

> B 

## column 

The physical location of the plasmid encoding this mutant, column number. (A lot of the boxes only have columns up to 9.)

Numerical index 

> 8 

## expression 

Does the mutant appear on a gel after 2 independent attempts to produce and purify? `1` for yes and `0` for no. 

`1` for yes, `0` for no 

> 0 

## gel_number 

The index of the gel that this mutant appears on. Gels for a given data set are labeled in order from 1. Gel images should be saved on the gel imaging computer completely labeled. Ladder should be labeled with its name, e.g. "Thermo PAGE-Rule". Mutants should be labeled with their names. Wild type proteins should be labeled as "WT". It's not necessary to further distinguish wild type proteins. 

Numerical index 

> 4

## protein_yield 

Protein yield as assessed by A280. 

mg/mL 

> 1.28

## kcat

## kcat_err 

## km

## km_err

## kcatkm 

## kcatkm_err

## tm

## tm_err

## data_complete 

Is the data for this mutant 100% correct and complete? 

`1` for yes and `0` for no (default: `0`) 

> 1

# FAQ 

## Why are all the names lowercased single words with underscores instead of spaces? 

The names are formatted this way for ease of use with pandas
