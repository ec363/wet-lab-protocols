# Electrocompetent cells

_Eszter. Adapted from UCL protocols. Rewritten 2019 March, 2019 Sept._

**Background**: Cells are grown to early log phase and harvested in this state to allow optimal recovery (expression of resistance gene(s)) before plating. The OD at harvest and the concentration of the aliquots are the key factors for efficiency. The entire protocol post-cell growth is simply a way to remove as much of the salt in the media as possible.

---

##### Starting materials:

1. overnight E. coli culture.
2. 1 M HEPES buffer pH 7.0 (commercial)

---

##### Protocol:

##### Day -1

**Media**

* morning (or earlier): make up (eg.) 400 ml(#) of LB directly into a large conical flask and take for autoclaving
    * Scale: if doing this for the first time, start with 200 ml.
    * Media. I've used 2TY and LB-Miller. It shouldn't matter too much unless the cells are fussy.
    * Reason: this is much cleaner than aliquoting 400 ml from a beaker of sterile LB.

* (#) __Consider Scale of Culture:__
    * 200 mL culture --> 40 aliquots
    * 400 ml --> 80
    * 800 ml --> 160
    * [These are overestimates.]
    * 200 ml will --> 1.5 ml final pellet volume = 50 µl x 30 aliquots max, by calculation, let alone in practice.
    * Although if you use 40% glycerol, you end up diluting this to 3 ml, which gives you 60 aliquots with slightly fewer cells in each.

**Buffer**

* more prep: 1 mM HEPES
    * Take a 500 ml filter sterilising plastic bottle. Add 500 ml deionised water to top compartment. Under flame, add 500 ul of 1 M HEPES. Filter the 500 ml (B609 has vacuum) and once done, give it a good shake to mix in the HEPES. Store in fridge and only open under flame.
    
**Cells**

* evening: grow up overnights for competent cells.
    * add antibiotic if relevant. otherwise just be very careful

##### Day 1

**Start Culture**

Start a fresh (< 3% inoculum v/v if applicable, I do 1%) well aerated (>=250 RPM) culture (culture volume =< 20% of flask volume to ensure good aeration) at 30 oC. Monitor bacterial growth at OD600 until it reaches 0.4 ~ 0.5.

* 30 oC recommended as cells grow slower and it’s less likely that you will “miss” the 0.4-0.5 window.
* The time it takes to reach it varies dependent on strain. Start measuring at 1h (stop culture, carefully under flame take 1ml -> cuvette and measure in spectrophotometer in B606), and continue until you find the 0.4-0.5 window.
* This is probably the most important factor in efficiency - where you stop the culture.
* If you’ve gone above 0.6, you will get low efficiency. It’s not good enough just to dilute it to 0.4 becuase the cells are too far into log phase. You need to dilute to 0.1 and then grow it again until 0.4. Or just start again.

**Stop Culture**

Transfer culture to ice for 10 minutes.

While you wait:

* find 2 ice boxes - 1 for HEPES, other for cells.
* take 1 mM filtered HEPES from fridge, into box1, surround with ice.
* take 50 ml falcon tubes, label with cell strain and stick them in box2 to pre-cool them.
* pre-chill the centrifuge to 4oC!

**Remove Media**

If you are working with 200 mL, use 4 Falcon tubes.

Split culture between as many falcon tubes as you need. I aliquot 45 ml per tube because you always lose a bit of volume to evaporation / taking OD readings, then make up all with spare cells and sterile LB at end. Need them to be at exact same volume to balance the centrifuge.

Harvest cells by centrifugation for 10 minutes at 4000 RPM (~935 g) at 4 oC.

**Wash cells 3x in HEPES**

Discard supernatant and resuspend cells in 1 mM HEPES. Add 5 mL of buffer to the cell pellet, leaving it on ice for 10 minutes before trying to resuspend the cells. The cells will be quite difficult to resuspend at this point but need to be resuspended as gently as possible (as lack of salt in the solution with steadly weaken cell wall) - best way is to flick with the palm of your hand.

Once resuspended, top up the buffer to 50 mL (# see below) and centrifuge (same conditions as before). Repeat the washing procedure two more times (i.e. discard supernatant and resuspend cells in fresh buffer).

(#) After each wash, you can start pooling cell fractions so that you go from 4 to 2 to 1 tube of cells. ie. You need to do 3 washes. The first spin is not a wash, so:

* grow cells (200ml) - 4 x 50 ml falcons. spin.
* resuspend in 5 ml. merge tubes 1+2 to make 10 ml, and add 40 ml HEPES. merge tubes 3+4 and add 40 ml HEPES. this is wash1. spin.
* resuspend in 5 ml. merge tubes 1+3 to make 10 ml, and add 40 ml HEPES. this is wash2. spin.
* resuspend in 5 ml. add 45 ml HEPES. this is wash3. spin.

The cells will become easier to resuspend after each wash. After the cells have been washed 3 times, resuspend the cell pellet in 1000 uL (flicking usually works, or very gentle vortex (strength 3 of 6). Pipetting can be harsh on cells due to shearing forces.

**Add glycerol, aliquot and freeze**

Once cells are resuspended, estimate their volume (probably around 1.3 ~ 1.5 ml), and **add glycerol (either 100% or 40% v/v) to a final concentration between 10% and 20%.** (I resuspend to 1.5 ml and add 1.5 ml 40% glycerol.) Gently mix. Samples are ready for use or for aliquoting.
 
To aliquot, place an aluminium block (from the heat blocks) in a shallow ice box with dry ice and allow 0.5 mL tubes to chill for 2 minutes before pipetting cells into the tubes, so that cells can flash freeze as soon as they are added to the tubes. Divide your cells in 50 uL aliquots. I usually transfer the cells from the block to a labelled plastic bag in the dry ice (thus saving on labelling every tube) and then transfer that to the -80oC as soon as it is convenient. Label should include: Your name and date, Cell strain, Aliquot size in ul, that it’s electrocompetent.
 
If you want to transform straight away, just transfer 50 uL of the cells directly to a pre-chilled electroporation cuvette.

Electroporation protocol:

* pre-chill electroporation cuvette
* Add 1 ul of 10ng/ul plasmid (different for ligation or Gibson mixtures)
    * to 50 ul cells
    * Do not pipette up/down
    * Just transfer straight into cuvette.
* No need to incubate on ice.
* Electroporate (Bacterial protocol, 1.8 kV. ms of 5.0 expected.)
* As quickly as possible, under flame, add 950 ul LB to cells
* Transfer all to 14 ml tube.
* Recover 37oC with shaking 30min (Amp) - 1h (others).
* Plate on 2 plates as 50ul or 200ul.

##### Day2

Check transformations worked.

Calculation of transformation efficiency in colony forming units (cfu) per ug DNA.

Best practice is to use the same plasmid for each of these tests so you can compare between batches, eg pUC19 or pBAD-GFP.

* Count colonies on plate or approximate.
* eg. if you used above protocol and plated 50ul
    * say you count 100 colonies
    * = 100 colonies / 50ul of culture / 10 ng DNA
    * = 2000 colonies / whole 1 ml recovery / 10 ng DNA
    * = 2000 cols/10ng
    * = 2 x 10^5 colonies / ug DNA

---
