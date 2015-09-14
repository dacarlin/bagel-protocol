# Production and purification of BglB

This is a guide to the production and purification of β-glucosidase B from *P. polymxa* beginning with purified plasmid and ending with purified protein. This protocol and the associated scripts and data in this repository are part of the [Siegel group](https://sites.google.com/site/ucdsiegellab/)'s "Bagel" project. 

For this procedure, typical yields are 1.0 ± 0.4 mg/mL for the wild type protein. 

Before beginning, make sure you have the following:

+ thermocyler or dry bath
+ 37 C standing and shaking incubators
+ centrifuge 
+ 

## Day 1: Transformation 

In this step, you will transform the plasmids encoding your mutant genes into *Escherichia coli BL21(DE3)*. Transformation is the process of physically shocking the bacteria to induce them to take up foreign DNA from the environment. Today, you will heat shock the *E. coli* to induce the uptake of the plasmid encoding the mutant you designed. 

Material | Concentration  | Amount per reaction
---------|----------------|--------------------
Chemically-competent *Escherichia coli* BL21(DE3) | | 30 μL 
Mutant plasmid solution | > 20 ng/μL | 2 μL
Terrific broth (TB) | | 200 μL
LB agar plates with kanamycin | | 1
Sterile glass beads | | 8–10 
2 mL tube | | 1

### Mise en place

+ waste bucket 
+ P2 and tips, P200 and tips
+ Ice in ice bucket
+ Pre-warmed 42 C dry bath or thermocycler

### Hardware

+ 37 C incubator

### Instructions 

1. Set 2 mL tubes on ice, one per mutant
2. When the tubes are ice cold, add plasmid and competent cells and incubate on ice for 10 minutes 
3. Heat shock at 42 C for 60 seconds 
4. Incubate on ice for 5 minutes 
5. Add 200 µL Terrific Broth and recover at 37 C for 1 hour
6. Pipet 200 µL recovered cells on to plate, add glass beads, shake, and get rid of beads
7. Incubate plate upside down overnight at 37 C

### Tips and tricks 

+ Chemical competent cells should be kept on ice at all times and never warmed
+ Program the thermocycler to perform steps 1-5
+ Some tips for [troubleshooting transformations from New England Biolabs](https://www.neb.com/tools-and-resources/usage-guidelines/chemical-transformation-tips) 


## Day 2: Growth 

Today, you will record the number of colonies on your selection plate and start a culture from a single colony. 

Material | Amount per reaction
---------|---------------------------
Transformation plate | 1
Terrific Broth | 5 mL
Kanamycin solution | 5 μL
Tube seal | 1

### Instructions 

1. Record the number of colonies on your transformation plate.  
2. Add kanamycin solution to Terrific Broth to make a batch of growth media for all of your mutants. Make enough for one extra culture. 
3. Aliquot 5 mL growth media to a Falcon tube 
1. Using a pipettor, carefully scrape a single colony from the plate and dip in the growth media in the Falcon tube while pipeting up and down to start the culture
2. Repeat for the other plates 
5. Seal the cultures with tube seals 
6. Incubate with shaking at 37 C for 24 hours


### Tips and tricks 

+ If you have a lot of colonies, divide the plate into quadrants, count one quadrant, and multiply the resultant number by 4 to estimate how many colonies you got.


## Day 3: Expression cultures 

In this step, you will exchange the spent growth media in your cultures with fresh growth media supplemented with IPTG. IPTG will induces expression of your target protein. 

Material | Amount per reaction
---------|---
Growth cultures from day 2 | 1
Terrific Broth | 5 mL
IPTG solution | 5 μL
Kanamycin solution | 5 μL
Tube seal | 1

_Minirecipe_: 5 mL induction medium = 5 mL Terrific Broth + 5 µL kanamycin solution + 5 µL IPTG solution

### *Mise en place*

+ tube rack
+ vortexer
+ P20 and tips
+ serological pipet and tips

### Hardware 

+ centrifuge
+ shaking incubator at 37 C 

### Instructions

1. Centrifuge growth cultures at 4,700 RPM for 10 minutes 
2. Peel the seals off and pour away supernatant from cell pellet 
3. Weigh the pellet and record your pellet weight 
4. Make a batch of induction media (make enough for n+1) 
1. Add 1 mL induction medium to cell pellet in tube 
1. Vortex to resuspend pellet
1. Add 4 mL more induction medium to tube
1. Seal with tube seals
1. Incubate with shaking at 18 C for 24 hours 

### Tips for today 

+ Devise a clever way to simplify resuspension 
+ [More information about how the pET expression system works](http://www.genomics.agilent.com/article.jsp%3FpageId%3D472)


## Day 4: Protein purification 

Today, you will purify the protein you designed for testing! 

Material | Amount per reaction
---------|-----------------------------
Expression culture from day 3 | 5 mL
Wash buffer | ~ 5 mL 
BugBuster | 50 μL
Dry lysis mix | 1 mg
2 mL tube | 1
Protein buffer | 200 μL
Ni-NTA resin slurry | 100 μL

### Hardware

+ centrifuge 
+ rocker 

### Mise en place 

+ waste bucket 
+ tube rack 
+ flow-through collector
+ microcolumns
+ P1000 and tips 

## Method 

_Minirecipe:_ 500 uL lysis buffer = 450 uL wash buffer + 50 uL 10X BugBuster + 1 mg dry lysis mix

1. Centrifuge expression cultures at 4,700 RPM for 10 minutes
2. While they are spinning, make lysis buffer
3. Useal culture and pour away supernatant 
4. Add 500 uL wash buffer to pellet and vortex to resuspend (should have about 1 mL in there) 
1. Aliquot 500 µL lysis buffer into resuspended pellets in 2 mL tubes
1. Rock tubes for 20 minutes 
1. Centrifuge at 14,700 RPM for 20 minutes to clarify the lysate 
1. While centrifuging, prep your microcolumns
2. Set cleaned microcolumns (if necessary, rinse with water) in rack over waste collector 
1. Add 100uL of nickel resin (blue) from 50% slurry to each microcolumn
1. Add 500 µL of wash buffer and allow to drip through
1. Once the lysed cultures have finished spinning, add 500 µL of clarified supernatant and allow to drip through 
1. Add another 500 µL of supernatant and allow to drip through  
1. Wash six times with 500 µL of wash buffer, allow to drip through each time, nice to have a repeater for this 
1. Once all unwanted proteins have been washed away, transfer column to fresh tube
1. Add 100 µL protein buffer directly to beads and incubate at room temperature for five minutes 
1. Add second 100 µL protein buffer and pulse in the centrifuge a couple of times to ensure you get all the liquid
1. Wash out the columns
2. Your purified protein is ready to quantitate by absorbance at 280, run on a gel, and use in an assay. 
3. Purified protein can be stored at 4 C for up to 48 hours before assay 
