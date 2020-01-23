# TypeIIS example protocol

Eszter Csibra

**Aim**: eg. to insert [gene seq for protein of interest (POI)] into [vector] for [protein expression].

---

### Type IIS
_From 2014-2016._

---

##### SUMMARY:

Vector

- [] Inverse PCR (iPCR) of **VECTOR** w [**primers**]  (#)
- Tm = **XX**; elongation = **XX**
- [] Check 5 µl of on gel
- [] DpnI digest of rest
- [] PCR purify
- [] Digest w [**Type IIs enzyme**]
- [] PCR purify

Insert

- [] PCR of **INSERT** w [**primers**]  (#)
- Tm = **XX**; elongation = **XX**
- [] Check 5 µl of on gel
- [] DpnI digest of rest
- [] PCR purify
- [] Digest w [**Type IIs enzyme**]
- [] PCR purify

Ligation

- [] Ligate
- [] Transform into 10beta cells.
- [] Check colonies possess correct plasmid. EITHER (A) or (B): A. Colony PCR w [**primers**] B. see after Minipreps.
- [] Minipreps
- [] Check colonies if not done A above. B. Digest w [**enzyme**] that will give you unique restriction pattern for cloned plasmid (that’s different from input vector). Chosen enzyme —> [**Expected results.**]
- [] Sequence w [**sequencing primers**] over any ligation sites.

- [] Analyse sequences - sort minipreps (keep/discard).
- [] Make sure plasmid is in correct strain for expression (eg. transform into T7 if IPTG induced construct).
- [] Make glycerol stocks.

---

##### DETAILS OF CERTAIN STEPS

**PCR**

Q5 reaction. See https://ec363.shinyapps.io/pcr_calc/ for recipe and cycling conditions.

Set up as many reactions as template/primer combinations, +1 for a negative control (no template). If you see a product here, this indicates contamination in one of your reagents. It's good practice to have a negative control for each primer set, as this controls for contamination in each primer set.

Make up the recipe as a master mix for several samples, adding the water first and enzyme last. Leave out the template. Aliquot 24 ul per 200 ul PCR tube, and add 1 ul template where relevant. Vortex, spin down, transfer to thermocycler.

Thermocycler notes: from experience, holding at 10 oC is better than 4 oC as some instruments can be badly damaged by holding at 4 oC, being opened and left on (as can happen). The water build up can damage the instrument. It shouldn't, but it does, so hold at 10 oC. DNA is pretty stable, and the enzyme will not be active.

-

**DpnI**

Protocol:

To the 20  ul remaining, add 1 ul DpnI, vortex to mix, spin reaction down in microfuge. Protocol in thermocycler can be copied from mine: 37 oC 45 min for the DpnI reaction, 80 oC 20 min to inactivate the enzyme, hold at 10 oC.

Information:

DpnI cuts at the very common site GA^TC. The utility of this enzyme results from its selectivity towards Dam methylated sites - a modification on plasmids isolated from bacteria with active Dam methylation systems but not in vitro (PCR) products. While it cuts both methylated and unmethylated DNA, it cuts methylated DNA 60X faster, so can be used to selectively get rid of plasmid DNA.

More on DpnI: https://international.neb.com/faqs/0001/01/01/what-s-the-difference-between-dpni-dpnii-mboi-and-sau3ai

More on methylation: https://international.neb.com/tools-and-resources/selection-charts/dam-dcm-and-cpg-methylation

-

**PCR purification**

Follow instructions in manual, elute in 30 ul elution buffer (Tris/EDTA).

-

**Type IIS enzyme digestion**

Protocol for AarI:

Reaction mixture:

* 30 ul DNA
* 5 ul 10X buffer
* 1 ul oligo
* 3 ul AarI
* 11 ul H2O

= 50 ul

Add water first, enzyme last, vortex to mix, spin down reaction.

Reaction conditions:

* 37 oC 3 h
* 65 oC 20 min to inactivate enzyme
* hold at 10 oC

-

**Ligation**

Basic reaction:

* _ µl Vector DNA [#]
* _ µl Insert DNA [#]
* 1 µl 10X T4 ligase buffer
* to 10 µl w mQ H2O.
* Incubate: 10’ at RT. [ie. can move onto transformation very quickly.]
* Alternative is 16oC overnight.

[#] It is usually recommended that you add about 1 vector:3 insert, in terms of molar ratio. And don’t add more than about 100ng DNA per 10 µl reaction to reduce non-specific ligation or self-ligation.

Typical set up for Type IIS reactions:

- **Reaction 1 is your ligation, L. As above.**
- **Reaction 2 is your control, C.** Leave out insert DNA. This controls for vector religation and/or colonies from any remaining input vector DNA. (Ideally you should get zero colonies.)

Thorough version:

Type IIS reactions typically work first time. If not, one can set up a range of V:I ratios:

- Ligation#1 (L1). V:I ratio = 1:1
- L2. V:I ratio = 1:3
- L3. V:I ratio = 1:10
- C. (control). Leave out insert DNA. 

-

**Colony PCR**

Colony PCR allows you to pick colonies straight into a PCR tube and find out whether the plasmid it’s carrying looks right. This requires you to have (or to design) primers that will give you useful information. Two good ways of doing it are:

1. Design primers within the vector sequence that flank the insertion site. In successful plasmids, they will give long PCR fragments (however long your insert is) and in unsuccessful ones a very short product (eg 100 bp).
2. Design primers where one anneals to insert and one anneals to vector. Correct plasmids will give predefined PCR fragment size, incorrect plasmids will give wrong size, or (more likely) no PCR product.

Set up Taq PCRs (high fidelity/speed is not paramount here). See https://ec363.shinyapps.io/pcr_calc/ for recipe and cycling conditions.

**Modifications: Once you pick a colony, you lose your only source of potentially-correct-plasmid-containing cells. In order to ‘save’ it, you have to streak it on another agar plate (a ‘master plate’). So the best order to do a colony PCR is:**

1. Decide on a sensible number of colonies to check. eg. 8.
2. Make up colony PCR master mix for 10 reactions (without template DNA, with Taq pol), and aliquot into (8) tubes.
    - **Make a 9th your negative control.**
3. Under a flame and in one go:
    - **For each colony: Pick colony, (a) streak on agar plate, (b) swirl in one of the PCR mixes and (c) add to 10 ml o/n culture.**
    - **Adding colony to o/n culture saves an entire day in the protocol**
    - Repeat for other colonies.
4. Thermocycler for PCR reaction.
    - **Extend initial denaturation (95oC) step to 5 min to ensure cells are lysed.**
5. Run agarose gel to check whether you have amplified the expected products.
6. Next day: mark up master plate to show which are good/bad. Grow up 2x good ones for miniprep and sequencing.


---
