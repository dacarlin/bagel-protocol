# Assay to determine kinetic parameters of BglB mutants 

This assay assumes that you have followed the protein production and purification steps in `production.md` in this repository. 

## Mise en place 

+ waste bucket 
+ pipet basin 
+ P200 and tips
+ Multi-channel P50 and tips
+ Multi-channel P300 and tips 

## Software 

Material | Amount per reaction |
---------|---------------------|
Diluted purified protein | 600 µL |
Substrate stock | 1800 µL |
Protein buffer |  |

## Instructions 

### Perform a qualitative test of the enzyme activity of your mutants 

1. For each mutant, label two 2 mL tubes
2. Mix 90 μL substrate stock and 10 μL purified protein
3. Wait five minutes for results 
3. If this turns yellow within five minutes:
   + make a 1/100 (100-fold) dilution: in the fresh tube, add 10 μL purified protein and 990 μL wash buffer
4. If this **does not** yellow within five minutes:
   + make a 1/10 (10-fold) dilution: in the fresh tube, add 100 μL purified protein and 900 μL wash buffer

Your diluted proteins will be used in the rest of the assay. You can store your purified protein at 4 C for up to 48 hours.  

### Prepare a substrate plate 

First, make the substrate plate. You can use any convenient plate for this, the $1 Costar full-area plates are best.
 
1. Using a single-channel pipet, dispense 150 μL of substrate stock into row A (12 wells) 
2. Using a multi-channel pipet, dispense 112.5 μL of protein buffer into rows B, C, D, E, F, G, H (the rest of the rows)
1. Using the multi-channel pipet, remove 37.5 μL from the first row and add to second row, and mix three times
3. Repeat this procedure for the second, third, forth, fifth, and sixth rows
4. Remove 37.5 uL from the seventh row, and throw away the liquid with the tips. Do not touch the last row in this step 
6. Verify that every well in the plate is the same volume (112.5 µL)

You have created a gradient of substrate concentrations in the substrate plate. 

### Prepare a protein plate 

Aliquot your proteins into the protein plate

1.  For each mutant, aliquot 25 µL of **diluted** purified protein into each well of three columns of the plate (24 wells in a 3x8 rectangle)

Now you have both substrate and protein (assay) plates ready to go. 

### Initiate assay and collect data 

Before you begin the instructions below, set the Gen5 software to the BglB assay. If you are setting up a Gen5 experiment file for the first time, see settings below. 

To initate the assay, transfer 75 µL from each well in the substrate plate into the protein plate.  

1.  Using the multichannel pipet, transfer 75 µL from the bottom row of the substrate plate into the bottom row of the assay plate
2.  Repeat for the rest of the rows (bottom up)
3.  Place the plate on the prepared plate reader and run the program 
4.  **Important**: fill out the "Information" panel (on the Gen5) with your name, the mutants you are testing, and the dilutions that you used. Use this format: 

> Alex Carlin. Cols 1-3: WT @ 100X, cols 4-6: E164A @ 10X, 7-9: I300L @ 100X, cols 10-12: E353A @ 10X

### Visual inspection of kinetic data  

+ Kinetic data points for this assay should lie on a straight line with positive slope
+ Slopes less than 1e-6 are probably not signficant 
+ The plate reader detector reads any OD higher than 3.75 as 3.75 under these conditions

Advice:

+ Visually assess R-squared values for the 96 rates on your plate (R-squared values closer to 1 are better)
+ Mask points as necessary to compensate for detector limit (OD 3.75) so you don't get artificially low reported rates 
+ Mask sparingly 

### Once you have verified your data 

4. [Fit your data to the Michaelis-Menten equation to determine kinetic parameters for your mutants](http://bagel.genomecenter.ucdavis.edu) 

### Gen5 setup 

Set up the Gen5 software that runs the Epoch and Synergy in the following way: 

+ run for 1 hour, full plate absorbance reading at 420 nm at 60 second intervals 
+ calculate maximum rate (MaxV [420]) based on 20 points 

These settings can be found under "Data Reduction > Calculation Options"

