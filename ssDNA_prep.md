# Production and isolation of BglB ssDNA 

## Day 1

Transformation of pET29b-BglB into E. coli K12 CJ236 **FΔ(HindIII)::cat (Tra+ Pil+ CamR)/ ung-1 relA1 dut-1 thi-1 spoT1 mcrA**

### Consumable materials 

+ chem competent CJ236 cells 
+ WT BglB plasmid 
+ selection plate containing 1X kanamycin and 1X chloramphenicol 
+ 15 mL round-bottom Falcon tube 

### Mise en place 

+ P1000 and tips 
+ plate
+ plasmid 
+ tube 
+ waste bukkette 

### Instructions

1. Transform as in `production.md` 
2. Make media for Day 2: autoclave 2, 250 mL flask with 50 mL TB 
3. Plate and incubate overnight at 37 C 

## Day 1: ssDNA Production (growth, virus inoculation, and overnight) 

### Consumable materials 

+ M13 phage (NEB) 
+ media made yesterday, 2, 250 mL flask with 50 mL TB
+ 2, 15 mL round-bottom tubes 

### Mise en place 

+ waste bucket
+ P20 and tips
+ serological pipet aspirator
+ 50 mL serological pipet

### Instructions

1. Dispense 3 mL into each tube 
1. Scrape 6 colonies into each tube 
2. Grow for 4-6 hours at 37 C with shaking until cloudy
3. Add 3 µL of M13K07 phage
4. Continue growing for 1 hour at 37 C with shaking 
5. Expand culture by diluting 1 mL from the tubes into the media in the flasks
6. Grow overnight at 37 C with shaking 

## Day 2: Harvesting ssDNA 

Materials | Concentration | Amount/ reaction
--------- | ------------- | ----------------
20% PEG   |     2.5 M      |       10 ml
1xPBS      |     n/a       |       2 ml (1st resuspension)
1xPBS     |     n/a       |       1 ml (2nd resuspension)
PEG/NaCl  |   n/a         |       2 ml
PNK Buffer  |     n/a     |       3 ul
ATP       |     10mM      |       1 ul
T4 Polynucleotide Kinase  |       n/a     |     1 ul
ddiH2O    |     n/a       |       18 ul


### Mise en place 

+ 50 ml Falcon tubes (x2)
+ Microfuge tubes
+ Pipette
+ PCR strip tubes or 96well PCR Plate

### Instructions

*Minirecipe:* KRM (n+2) = 3ul PNK Buffer + 1ul ATP + 1ul T4 Polynucleotide Kinase + 18ul ddih2O

1. Spin down overnight culture in sterile 50ml Falcon tube at 7000rpm for 20 minutes at 40C.
2. Transfer supernatant (contains phage) to a new sterile 50ml Falcon tube. 
3. Add 10ml 20% PEG/2.5M NaCl and mix thoroughly and incubate on ice for 45 minutes.
4. Spin down the phage at 7000rpm for 20 minutes at 40C.
5. Decant liquid and let tube stand upright to drain off the rest of the liquid. 
6. Resuspend the pellet in 2ml 1xPBS. Vortexing is okay.
7. Spin at 14,000rpm for 5 minutes.
8. Transfer the supernatant to new microfuge tubes with 300ul PEG/NaCl.
9. Vortex and incubate at room temperature for 10 minutes. 
10. Spin down phage at 14,000rpm for 2 minutes. 
11. Pipette off supernatant. Do a second quick spin to collect residual liquid and pipette it off.
12. Resuspend the pellet (phage) in 1ml 1xPBS.
13. Spin down at 14,000rpm for 5 minutes.
14. Transfer the supernatant (phage) to a new microfuge tube.
15. Harvesting ssDNA from Phage using Qiagen Qiaprep M13 kit (#27704)
    * DO NOT SPIN OVER 8000rpm when using this kit!
  
### Evaluation, tips, and tricks 

If A260 implies DNA concentration is below 20 ng/µL the procedure likely didn't work. 

Run a gel to make sure you can see a clear band. The pET29-BglB construct is ~6700 bp. Single-stranded DNA runs about 10% faster on a gel than supercoiled double-stranded DNA. 

## Recipes

### salt PEG (20% PEG/2.5M NaCl, 1 L) 

+ 200g PEG (polyethylene glycol) 8000MW
+ 141.6g NaCl
+ Add dH20 to 1L
+ Autoclave with a stir bar, stir immediately after autoclaving until cool, and store at 40C.

### phosphate-buffered saline (PBS, 1 L) 

+ 800 mL water
+ 8g NaCl
+ 0.2g KCl
+ 1.44g Na2HPO4 sodium phosphate 
+ 0.24g KH2PO4 potassium phosphate 
+ Adjust pH to 7.4
+ Add water to 1 L
