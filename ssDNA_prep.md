# Production and isolation of BglB ssDNA 

Adapted from the procedure in [Zhou 2009](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC2692612/)

## Day 1

Transformation of pET29b-BglB into E. coli K12 CJ236 *FΔ(HindIII)::cat (Tra+ Pil+ CamR)/ ung-1 relA1 dut-1 thi-1 spoT1 mcrA*

### Consumable materials 

+ chem competent CJ236 cells 
+ WT BglB plasmid 
+ selection plate containing 1X kanamycin and 1X chloramphenicol 
+ 15 mL round-bottom Falcon tube 

### Mise en place 

+ waste bucket 
+ P200, P1000 and tips 

### Instructions

1. Transform as in `production.md` 
2. Make media for Day 2: autoclave 2, 250 mL flask with 50 mL TB 
3. Plate and incubate overnight at 37 C 

## Day 2

ssDNA Production (growth, virus inoculation, and overnight) 

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

## Day 3

Harvesting ssDNA and evaluation of the procedure. 

> The phage particles produced in a 50 ml overnight culture of JM109/pGEM5Z(+)-EGFP/M13KO7 complex were recovered from the supernatant by the classical PEG precipitation procedure [6] and lysed in 2 ml of a disruption buffer (5 M Guanidinium Hydrochloride, 1% Triton X-100, and 10 mM MOPS, pH 6.5) with a short incubation of 5 min at room temperature. A silica column (Tiangen Biotech Co., LTD, Beijing, China) with a maximum DNA adsorption quantity of 500 μg was placed inside a 50-ml Falcon tube. The cell lysate was poured into the column, which was then centrifuge at 10,000g for 2 min. The flow-through solution was discarded and the column was washed twice with 5 ml of 80% isopropanol and centrifugation at 10,000g for 2 min. The column was then transferred to a new Falcon tube and incubated with 1 ml of sterile TE buffer for 2–3 min to elute the bound DNA. The eluted DNA in the TE buffer was collected by centrifugation at 10,000g for 2 min. The 50 ml culture usually yielded a total 150–200 μg ssDNA

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

All centrifugation steps at 4 C 

1. Spin down overnight culture in 50 mL tube at 4700 RPM for 20 min
2. Aliquot 10 mL salt PEG to fresh 50 mL tubes 
2. Transfer supernatant (contains phage) to fresh tubes 
3. Vortex and incubate on ice for 45 min
4. Spin down the phage at 4700 RPM for 45 min
5. Decant liquid and let tube stand upright to drain off the rest of the liquid
6. Resuspend the pellet in 2 mL PBS by vortexting or pipeting 
7. Spin at 14,000 RPM for 5 min
8. Transfer the supernatant to new microfuge tubes with 300 µL salt PEG 
9. Vortex and incubate at room temperature for 10 min
10. Spin down phage at 14,000 RPM for 2 min
11. Pipet supernatant off pellet
12. Do a second quick spin to collect residual liquid and pipet it off
12. Resuspend the pellet (phage) in 1 mL PBS 
13. Spin down at 14,000 RPM for 5 min 
14. Set centrifuge to 8,000 RPM  
14. Transfer the supernatant (phage) to a new microfuge tube
15. Purify using Qiagen M13 kit, **do not spin over 8,000 RPM**
  
### Evaluation, tips, and tricks 

If A260 implies DNA concentration is below 20 ng/µL the procedure likely didn't work. Run a gel to be sure, or just try again. 

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

### disruption buffer 

+ 5 M Guanidinium Hydrochloride
+ 1% Triton X-100
+ 10 mM MOPS
+ pH 6.5
