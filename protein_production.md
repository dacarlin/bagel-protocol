# Production and purification of BglB

This is a guide to the production and purification of β-glucosidase B from *P. polymxa* beginning with purified plasmid and ending with purified protein. This protocol and the associated scripts and data in this repository are part of the [Siegel group](https://sites.google.com/site/ucdsiegellab/)'s "Bagel" project. 

For this procedure, typical yields are 1.0 ± 0.4 mg/mL for the wild type protein. 

Before beginning, make sure you have the following ready and standing by:

+ dry bath set to 42 C
+ 37 C standing, 37 C shaking, and 18 C shaking incubators
+ centrifuges for 50 mL Falcon tubes (up to 4,700 RPM) and 2 mL tubes (up to 14,700 RPM) 

## Mise en place

*Mise en place* is a French culinary phrase which means "put in place", as in "set up". It is used in professional kitchens to refer to organizing and arranging the ingredients that a cook will require for the items that are to be prepared during a shift ([Wikipedia](https://en.wikipedia.org/wiki/Mise_en_place)). 

## Day 0: Kunkel mutagenesis 

After we have designed our set of mutants, we mutate the wild type Bagel plasmid to your designed sequence using [Thomas Kunkel's original procedure](http://www.pnas.org/content/82/2/488.full.pdf) or [our group's manual Kunkel protocol](https://docs.google.com/a/ucdavis.edu/folderview?usp=sharing&id=0B3zIXvOOrmpqcEM5WWRadThsVUE). If you're interested, historically orders were carried out on Transcriptic's cloud lab platform (see [Python code that automates the Kunkel procedure and algorithmicly evaluates sequence verification](https://github.com/dacarlin/bagel-orders)). 

## Day 1: Transformation 

In this step, you will transform the plasmids encoding your mutant genes into *Escherichia coli BLR(DE3)*. Transformation is the process of physically shocking the bacteria to induce them to take up foreign DNA from the environment. Today, you will heat shock the *E. coli* to induce the uptake of the plasmid encoding the mutant you designed. 

Material | Concentration  | Amount per reaction
---------|----------------|--------------------
Chemically-competent *Escherichia coli* BL21(DE3) | | 25 μL 
Mutant plasmid solution | > 20 ng/μL | 1 μL
Terrific broth (TB) | | 200 μL
LB agar plates with 50 µg/µL kanamycin | | 1
Sterile glass beads | | 8–10 
15 mL round-bottom culture tube | | 1

### Mise en place

+ waste bucket 
+ rack for 15 mL tubes 
+ P2 and tips,
+ P200 and tips
+ ice in ice bucket
+ pre-warmed dry bath (42 ˚C) 
+ agar plates 

### Instructions 

1. Dispense 1 µL aliquots of your mutant plasmid into the round-bottom tubes 
1. Set round-bottom tubes on ice and incubate on ice for 5 minutes 
2. While the tubes are chilling, get competent cells from freezer and set on ice
2. When the tubes are ice cold, add competent cells and incubate on ice for 15 minutes  
3. Heat shock at 42 C for 90 seconds 
4. Incubate on ice for 90 seconds 
5. Add 200 µL Terrific Broth and recover with shaking at 37 C for 1 hour 
6. Label the plates and place in incubator upside down to warm them 
7. Right before the hour is up, add glass beads to each plate
6. Pipet 200 µL recovered cells on to plate and shake to spread out the cells
7. After waiting a minute so that the liquid is absorbed, turn the plates upside down so that the beads fall onto the underside of the lid, and deposit beads into bleach solution for later recovery
7. Incubate plate *upside down* overnight at 37 C

### Tips and tricks 

+ Chemical competent cells should be kept on ice at all times and never warmed
+ Bring the ice bucket to the freezer 
+ Program the thermocycler to perform steps 1-5
+ Some tips for [troubleshooting transformations from New England Biolabs](https://www.neb.com/tools-and-resources/usage-guidelines/chemical-transformation-tips) 
+ If you are getting poor transformation efficiency, try recovering with 400 µL of media for 2 hours at 37 ˚C

## Day 2: Growth 

Today, you will record the number of colonies on your selection plate and start a culture from a single colony. 

Material | Amount per reaction
---------|---------------------------
Transformation plate | 1
Terrific Broth | 5 mL
Kanamycin solution | 5 μL
Tube seal | 1
50 mL Falcon tube | 1 

### Mise en place 

+ 50 mL tube rack 
+ waste bucket 
+ pre-cut seals
+ P1000 and tips 
+ serological pipet aspirator 
+ 25 mL serological pipet

### Instructions 

1. Record the number of colonies on your transformation plate 
2. Add kanamycin solution to Terrific Broth to make a batch of growth media for all of your mutants. Make enough for one extra culture
3. Aliquot 5 mL growth media to each 50 mL Falcon tube 
1. Using a pipet, carefully scrape a single colony from the plate and dip in the growth media in the Falcon tube, and pipet up and down a few times to inoculate the culture 
5. Seal the cultures with tube seals (cut into small squares first) 
6. Incubate with shaking at 37 ˚C for 24 hours

### Advice  

+ If you have a lot of colonies, divide the plate into quadrants, count one quadrant, and multiply the result by 4 to estimate the number of colonies 


## Day 3: Expression cultures 

In this step, you will exchange the spent growth media in your cultures with fresh growth media supplemented with [isopropyl β-D-1-thiogalactopyranoside](https://en.wikipedia.org/wiki/Isopropyl_β-D-1-thiogalactopyranoside) (IPTG). IPTG induces expression of your target protein using the engineered [pET expression system](http://www.genomics.agilent.com/article.jsp%3FpageId%3D472). 

Material                      | Amount per reaction
------------------------------|---
growth cultures from day 2    | 1
Terrific Broth                | 5 mL
1000x IPTG solution           | 5 μL
1000x kanamycin solution      | 5 μL
tube seal                     | 1

_Minirecipe_ (for 1 sample): 5 mL induction medium = 5 mL Terrific Broth + 5 µL kanamycin solution + 5 µL IPTG solution
_Minirecipe_ (for 4 samples) : 25 mL induction medium = 25 mL Terrific Broth + 25 µL kanamycin solution + 25 µL IPTG solution

### *Mise en place*

+ tube rack
+ vortexer
+ P20 and tips
+ serological pipet and tips

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

+ The more you observe sterile technique, the better the cultures will grow 
+ **Challenge**: Devise a clever way to simplify resuspension so that a robot could do it

## Day 4: Protein purification 

Today, you will purify the protein you designed for testing using a technique called *immobilized metal ion chromatography*. 

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

_Minirecipe (for 1 sample):_ 500 uL lysis buffer = 450 uL wash buffer + 50 uL 10X BugBuster + 1 mg dry lysis mix

_Minirecipe (for 4 samples):_ 2000 uL lysis buffer = 1800 uL wash buffer + 200 uL 10X BugBuster + 5 mg dry lysis mix

### Purification 

1. Centrifuge expression cultures at 4,700 RPM for 10 minutes
2. While they are spinning, make lysis buffer and set on rocker
3. Unseal culture and pour away supernatant 
4. Weigh your expression pellet and record the pellet weight
4. Add 500 uL wash buffer to pellet and vortex to resuspend (should have about 1 mL in there) 
5. Aliquot the resuspended pellets to fresh 2 mL tubes 
1. Aliquot 500 µL lysis buffer into resuspended pellets in 2 mL tubes
1. Rock tubes for 30 minutes at room temperature to lyse cells 
1. Centrifuge at 14,700 RPM for 30-60 minutes to clarify the lysate 
1. While centrifuging, prep your microcolumns. Set cleaned microcolumns (if necessary, rinse with water) in rack over waste collector 
1. Add 100 µL Ni-NTA resin slurry to bed of each microcolumn
1. Add 500 µL wash buffer and allow to drip through
1. Once the lysed cultures have finished spinning, add 500 µL of clarified supernatant and allow to drip through 
1. Add another 500 µL of supernatant and allow to drip through  
1. Wash six times with 500 µL of wash buffer, allow to drip through each time
1. Once all unwanted proteins have been washed away, transfer column to fresh tube
1. Add 150 µL protein buffer directly to beads and incubate at room temperature for 1 minute 
1. Add second 150 µL protein buffer and pulse in the centrifuge a couple of times to ensure you get all the liquid
3. Remove column from tube. Tube contains purified protein solution
1. Wash out the columns with DI water 
2. Your purified protein is ready to quantitate by absorbance at 280, run on a gel, and use in both kinetic and thermal stability assays

