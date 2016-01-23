# Production and purification of BglB

This is a guide to the production and purification of β-glucosidase B from *P. polymxa* beginning with purified plasmid and ending with purified protein. This protocol and the associated scripts and data in this repository are part of the [Siegel group](https://sites.google.com/site/ucdsiegellab/)'s "Bagel" project. 

For this procedure, typical yields are 1.0 ± 0.4 mg/mL for the wild type protein. 

Before beginning, make sure you have the following:

+ thermocyler or dry bath
+ 37 C standing and 37 C and 18 C shaking incubators
+ centrifuge for 50 mL Falcon tubes and 2 mL tubes 

## Day 0: Automated Kunkel mutagenesis 

After you have designed your set of mutants, an automated Kunkel mutagenesis procedure will be carried out on [Transcriptic](https://www.transcriptic.com/)'s workcell. The wild type Bagel plasmid is mutated to your designed sequence using the procedure that's described in [Thomas Kunkel's original procedure](http://www.pnas.org/content/82/2/488.full.pdf) and in [our group's manual Kunkel protocol](https://docs.google.com/a/ucdavis.edu/folderview?usp=sharing&id=0B3zIXvOOrmpqcEM5WWRadThsVUE). If you're interested, the [Python code that automates the Kunkel procedure and algorithmicly evaluates sequence verification](https://github.com/dacarlin/bagel-orders) is together but still a little messy (could use a second set of eyes on it).

After your mutant plasmids have been Kunkel'd and sequenced, you'll get them in the mail ready for Day 1.

### When you get your mutants 

**Note**: Everybody's mutants arrive together in a 96-well plate along with a CSV file that tells you where each mutant is on the plate. 

Material | Concentration  | Amount per reaction
---------|----------------|--------------------
2 mL tube | | 1
tube label | | 1

#### Mise en place

*Mise en place* is a French culinary phrase which means "putting in place", as in "set up". It is used in professional kitchens to refer to organizing and arranging the ingredients that a cook will require for the items that are to be prepared during a shift. ([Wikipedia](https://en.wikipedia.org/wiki/Mise_en_place))

+ waste bucket 
+ P200 and tips

#### Instructions 

1. Find your mutant in the CSV file (make sure to verifiy the plate barcode matches the sheet)
2. Write the mutant name on a ToughTag tube label and affix to a 2 mL tube 
2. Once you know which well your mutant is in, pipet the entire volume of that well into the tube
3. Store your mutants at -20 C in the "Bagel" box or go immediately to Day 1

## Day 1: Transformation 

In this step, you will transform the plasmids encoding your mutant genes into *Escherichia coli BL21(DE3)*. Transformation is the process of physically shocking the bacteria to induce them to take up foreign DNA from the environment. Today, you will heat shock the *E. coli* to induce the uptake of the plasmid encoding the mutant you designed. 

Material | Concentration  | Amount per reaction
---------|----------------|--------------------
Chemically-competent *Escherichia coli* BL21(DE3) | | 30 μL 
Mutant plasmid solution | > 20 ng/μL | 2 μL
Terrific broth (TB) | | 200 μL
LB agar plates with kanamycin | | 1
Sterile glass beads | | 8–10 
15 mL round-bottom culture tube | | 1

### Mise en place

+ waste bucket 
+ P2 and tips, P200 and tips
+ Ice in ice bucket
+ Pre-warmed 42 C dry bath 

### Hardware

+ 37 C incubator

### Instructions 

1. Set round-bottom tubes on ice, one per mutant
2. When the tubes are ice cold, add plasmid and competent cells and incubate on ice for at least 10 minutes (20 min is better) 
3. Heat shock at 42 C for 90 seconds 
4. Incubate on ice for 90 seconds 
5. Add 200 µL Terrific Broth and recover with shaking at 37 C for 1 hour
6. Place plates in incubator upside down to warm them
7. Right before the hour is up, add glass beads to each plate
6. Pipet 200 µL recovered cells on to plate and shake to spread out the cells
7. After waiting a minute so that the liquid is absorbed, turn the plates upside down so that the beads fall onto the underside of the lid, and deposit beads into bleach solution for later recovery
7. Incubate plate *upside down* overnight at 37 C

### Tips and tricks 

+ Chemical competent cells should be kept on ice at all times and never warmed
+ Program the thermocycler to perform steps 1-5
+ Some tips for [troubleshooting transformations from New England Biolabs](https://www.neb.com/tools-and-resources/usage-guidelines/chemical-transformation-tips) 
+ If you are getting poor transformation efficiency, try recovering with 500 µL of media

## Day 2: Growth 

Today, you will record the number of colonies on your selection plate and start a culture from a single colony. 

Material | Amount per reaction
---------|---------------------------
Transformation plate | 1
Terrific Broth | 5 mL
Kanamycin solution | 5 μL
Tube seal | 1

### Mise en place 

+ 50 mL tube rack 
+ waste bucket 
+ pre-cut seals
+ pipets and tips 
+ markers 
+ serological pipet aspirator 
+ 25 mL serological pipet

### Instructions 

1. Record the number of colonies on your transformation plate 
2. Add kanamycin solution to Terrific Broth to make a batch of growth media for all of your mutants. Make enough for one extra culture
3. Aliquot 5 mL growth media to a Falcon tube 
1. Using a pipet, carefully scrape a single colony from the plate and dip in the growth media in the Falcon tube, and pipet up and down a few times 
2. Repeat for the other plates 
5. Seal the cultures with tube seals 
6. Incubate with shaking at 37 C for 24 hours

### Tips and tricks 

+ If you have a lot of colonies, divide the plate into quadrants, count one quadrant, and multiply the resultant number by 4 to estimate how many colonies you got


## Day 3: Expression cultures 

In this step, you will exchange the spent growth media in your cultures with fresh growth media supplemented with [isopropyl β-D-1-thiogalactopyranoside](https://en.wikipedia.org/wiki/Isopropyl_β-D-1-thiogalactopyranoside) (IPTG). IPTG induces expression of your target protein. [Molecular details of how the expression system works](http://www.genomics.agilent.com/article.jsp%3FpageId%3D472). 

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

+ **Challenge**: Devise a clever way to simplify resuspension so that a robot could do it

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
