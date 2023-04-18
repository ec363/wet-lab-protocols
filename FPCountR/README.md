# FPCountR experimental protocol

Eszter Csibra

Equivalent to:

- Supp Note 5 in 2022 Csibra & Stan  
- V2 of FPCount in-lysate protocol on protocols.io

---

FPCount is a complete protocol for fluorescent protein calibration, consisting of:

1.	FP expression and production of cell lysates.
2.	FP concentration determination in a microplate reader.
3.	FP fluorescence quantification in a microplate reader.

Results can be analysed with the corresponding R package, FPCountR.

This in-lysate version of the protocol uses the ECmax protein quantification protocol of FPs in lysates and does not require His-tag purification of the FPs. Note that it is only suitable for FPs with entries in FPbase (https://www.fpbase.org/). 

CALIBRANT PREPARATION

Step 1. Expression

Set up a 50ml culture for the overnight expression of the calibrant fluorescent protein.

Mix the following in a 200ml flask:

- 50ml culture medium (such as LB Miller)
- 50µl chloramphenicol
- 50µl 20% arabinose (for a final concentration of 0.02%)
- scraping of an expression vector for the calibrant FP in an E. coli  strain suited to overexpression (e.g. pS381_ara_His-mCherry in E. coli BL21 strain)

Incubate the cultures at 30oC overnight with 250 rpm shaking.

Step 2. Harvesting and Washing

Harvest the E. coli after the overnight culture and wash them to remove media and exchange the buffer to a cell lysis buffer suitable for protein stability. For FPs that express to high levels (e.g. all three FPs from the vectors described in the paper), 20 OD600 units worth of cells contains enough protein for a calibration. For poorly expressing FPs, this can be increased (e.g. to 40 OD600 units of cells), for which users should adjust the relevant quantities below as required.

Prepare the following buffers:

- Wash buffer = T50N300 (50 mM Tris-Cl pH 7.5, 300 mM NaCl). About 10ml per FP required.
- Resuspension buffer = T50N300+pi (T50N300 with protease inhibitors). About 10ml per FP required.
	- Protease inhibitors (EDTA-free, Pierce A32955) are added to the buffer at 1 tablet per 10ml. As these dissolve poorly, it is important to filter sterilise the resultant solutions.
	- Lysis Buffer = T50N300+pi with 100µg/ml lysozyme. 2ml per FP required (if using 20 OD600 units of cells).
- The following should be available but not pre-prepared into buffers:
	- DNase I (1000U/ml in ddH2O)
	- a stock of CaCl2
	- a stock of MgCl2 

Procedure:

- Prechill (for 15min) 1x 50ml falcon tube per FP on ice for cooling the cultures
- Prechill 1x 50ml falcon tubes per FP on ice for sonication (1x falcon tube required per 20 OD600 of cells)
- Prechill a centrifuge with the ability to spin 50ml falcon tubes to 4oC
- Remove culture from incubator. For some FPs it will be clear by eye if expression levels are good.
- Transfer culture to the prechilled falcon tube on ice and cool for 20min. (From here on, cultures and proteins should be kept on ice and spun at 4oC unless otherwise stated.)
- Measure the culture OD600 (use 100µl of culture diluted 1:10 in culture medium) and calculate the OD600 of the original culture.
- Calculate the volume of culture to be aliquoted into the tube for sonication (equivalent of 20 OD600 worth of cells).

Example OD calculation:

|                | OD (cm-1ml-1) (1:10 dilution) | OD (cm-1ml-1) (neat culture) | total OD (ODml-1 * 50ml) | fraction of culture  that is 20 OD | volume (ml)  for 20 OD |
|----------------|-------------------------------|------------------------------|--------------------------|------------------------------------|------------------------|
|     mCherry    |     0.418                     |     4.18                     |     209                  | 0.096                              | 4.78                   |

- Add 20 OD to the prechilled tube set aside for aliquoted cultures. (The original cultures can be stored at 4oC for the day or be disposed of.)
- Pellet cells by spinning at ~3,220xg, 10min, 4oC
- Resuspend cells in 5ml Wash Buffer, then add another 5ml Wash buffer
- Pellet cells by spinning at ~3,220xg, 10min, 4oC
- Resuspend in 2ml (for 20 OD) Lysis Buffer (to final concentration of 10 OD/ml). 

Step 3. Lysis.

Lysis by sonication was found to give the most reliable results. This lysis protocol uses a QSonica Q125 sonicator; settings for other sonicators may vary.

- Stand falcon in small plastic beaker full of ice.
- Lower sonicator tip into the sample.
- Sonicate with settings: amplitude: 50%, pulses: 10s on/10s off, duration: 2min. 
- (NB. A 2min duration means 2 minutes of sonication. As this is carried out in pulses of 10s sonication followed by 10s of rest, this takes 4min.)

The lysed solution should go from turbid to clear. 

DNase I treatment: DNase treatment is essential if using A280 assay but may not be required for the ECmax assay (this hasn’t been tested). Note that DNase I is 31 kDa: similar in size to FPs in a way that may affect yield estimates in an SDS-PAGE, and is sensitive to vortexing.

- To lysates in Lysis Buffer, add: 
	- DNase I to 50 U/ml final
	- CaCl2 to 5mM final (13mM ideal for DNase I, <5mM recommended with His resins, 11)
	- MgCl2 to 50mM final
- Mix thoroughly
- Incubate for 30min at 4oC

Step 4. Clarification

Separate the insoluble fraction from the soluble proteins by centrifugation.

- Transfer lysates from falcons into pre-chilled 1.5ml Eppendorf tubes.
- Spin samples in pre-chilled microfuge at 16,000xg for 30min at 4oC.
- Transfer the supernatant (soluble) fractions to new 1.5ml Eppendorf tubes. Insoluble fractions (1 per FP) may be kept for checking by SDS-PAGE if desired.

Step 5. Protein concentration (optional)

In principle, lysates may not always need to be concentrated prior to calibration, but in practice it is recommended to ensure that there is a high enough concentration in the first few dilutions to get accurate protein concentration measurements from the absorbance readings. The total volume of lysate required may in some cases require trial and error, but 1.6ml (equivalent of 16 OD cells) is a good starting point. If 40 OD cells were lysed, up to 4ml lysate can be concentrated at this step. Another good rule of thumb (for green and red FPs at least) is that the FP stock should be concentrated enough to produce visibly colourful solutions.

Using Amicon Ultra 10K columns with 500µl capacity (Merck, UFC5010):
- Add lysate (400µl) to 10K Amicon column (1/n) 
- Concentrate by spinning at 14,000xg for 10min at 15oC
- Discard flowthrough
- Repeat the above 3 steps as many times as needed. (e.g. n = 4 for 1.6ml lysate)
- Recover resultant sample (~100µl) by eluting into a fresh tube (at 1,000xg for 1min) 

CALIBRATION

Step 6. Preparation of FP dilution series
A calibration plate should be prepared as a serial two-fold dilution series using the same type of 96-well microplate as used for the assays requiring calibration. (If assays are typically conducted using black plates, calibrations should be carried out using the same type of plate.) The requirements for the calibration are 100µl of a concentrated solution of each FP to be calibrated, about 6ml T50N300+pi buffer for each FP, and access to each plate reader to be calibrated. A single dilution series of protein can be used for both the protein assay and the activity assay, and this plate can be stored at 4oC if necessary.

Prepare serial dilution in 1.5ml Eppendorf tubes
Dilution series are best prepared in 1.5ml Eppendorf tubes as these are easier to handle (and see into) than wells of a deep well plate, which is important for avoiding errors.

A typical dilution series may be prepared as follows.

- Label 11 tubes (e.g. ‘mCherry 1’ to ‘mCherry 11’)
- Add 900µl T50N300+pi buffer to tube 1, and 500µl buffer to tubes 2-11.
- Add 100µl concentrated lysate to tube 1 and thoroughly mixed by vortexing and spinning or extensive pipetting.
- 500µl of lysate in tube 1 is removed and mixed (pipetting up and down carefully 8x) into tube 2. This is repeated from tube 2 to tube 3, etc, until tube 11.

Transfer dilutions into 96-well microplate

- Arrange plate with each FP occupying a pair of rows (e.g. mCherry in A/B, mGFPmut3 in C/D, etc.). Highest FP concentrations will be placed in the left column (column 1), the lowest near the right (column 11) and buffer in column 12.
- Fill wells in column 12 with 225µl T50N300+pi buffer.
- Transfer 2x 225µl from each FP dilution to the two corresponding wells of the microplate.
- Temporarily cover the plate with a removable lid to prevent it being contaminated (do not seal).

Example plate arrangement (d1 = dilution1 with highest concentration):

|          | 1  | 2  | 3  | 4  | 5  | 6  | 7  | 8  | 9  | 10  | 11  | 12     |
|----------|----|----|----|----|----|----|----|----|----|-----|-----|--------|
| mCherry  | d1 | d2 | d3 | d4 | d5 | d6 | d7 | d8 | d9 | d10 | d11 | buffer |
|          | d1 | d2 | d3 | d4 | d5 | d6 | d7 | d8 | d9 | d10 | d11 | buffer |
| mGFPmut3 | d1 | d2 | d3 | d4 | d5 | d6 | d7 | d8 | d9 | d10 | d11 | buffer |
|          | d1 | d2 | d3 | d4 | d5 | d6 | d7 | d8 | d9 | d10 | d11 | buffer |

Step 7. The ECmax assay (quantification of FP concentration)

- Prewarm the microplate reader to the temperature used for standard assays to make sure the calibrations are valid for those temperatures (e.g. 30oC).
- Insert the calibration plate without the lid and equilibrate the calibrants to the plate reader temperature.
- Take an absorbance scan of all filled wells between 200-1000nm. (Wavelengths above 900nm are required for path length correction. Other wavelengths are required for calculation of FP concentration, though UV wavelengths (<300nm) are not always necessary for FPs that absorb at longer wavelengths.)

Step 8. The fluorescence assay (quantification of FP activity)

- Remove the plate from the plate reader and seal the plate with a clear plastic seal (e.g. Eppendorf Masterclear real-time PCR film adhesive, 30132947).
- Take fluorescence scans on each plate reader requiring calibration and for each filter set that is used for that FP. Each scan should consist of fluorescence intensity detection at a range of gains (on Tecan Spark gains 40, 50, 60, … 120 are recommended) to allow the relevant scripts to calculate conversion factors for any gain.

Step 9. Storage of calibrants and calibration plates

Calibrants should be stored in the fridge, protected from light, where they should be stable for a few weeks after preparation. Calibrant functionality after longer term storage or after freeze-thaw cycles have not yet been tested.

Step 10. Analysis of calibrations

The aim of this protocol is to produce conversion factor(s) for any given FP that relate the number of FP molecules to the 'relative' fluorescence units (RFU) observed in a given instrument, with a given filter set, and gain. The previous steps described how to prepare lysates containing FPs to produce calibrants, and how to run the assays that quantify how many FP molecules there are in each well, and the RFU output of each well. This data must now be analysed to obtain the conversion factors required. 

The analysis should be carried out using FPCountR, an open-source R package we developed for this purpose. Functions in this package are provided for each analytical step. The parser() functions convert raw plate reader data into tidy data formats. The get_conc_ECmax() function calculates FP concentrations from the absorbance data. The generate_cfs() function obtains conversion factors using concentration and fluorescence data. Finally, process_plate() and calc_percell() functions extract data from microbial growth curves in units of molecules, and molecules per cell.

Validation steps and controls

Expression

- For some FPs (particularly bright greens and reds), it will be clear by eye if expression levels are high after overnight culture, as the culture will be brightly coloured. If this is not visible in the culture itself, it can become apparent after the first wash step as a brightly coloured cell pellet. For some of these proteins, the absence of colour typically means the expression conditions need optimisation. (Note that some FPs, such as mTagBFP2, will not produce a visible colour.)
- Overnight expression should produce high levels of protein but should not kill the cells: if using a plasmid that results in poor growth (less than 20 OD600 units of cells after overnight culture), use a lower inducer concentration, a lower growth temperature, or some other means to reduce cellular burden.
- Expression should result in adequate to decent yields of soluble protein and minimal aggregated protein. We do not see aggregation with our FPs, although in principle this can be a problem in protein overexpression that would limit FP yields. The presence of aggregates can be checked by SDS-PAGE after the clarification step that separates the soluble and insoluble fraction. The presence of a prominent FP-sized band in the insoluble fraction could indicate protein aggregation. This can often be resolved by using a lower inducer concentration or a lower growth temperature.
- The method has been validated with plasmids that are available on Addgene. These can be used as positive controls if users’ own plasmids do not produce enough protein or produce unexpected results.

Calibrant preparation

- The lysed solution should go from turbid to clear. If it doesn’t, this suggests the lysis was inefficient: repeat the lysis or increase the sonication amplitude or time.
- The clarification step that separates the soluble proteins from the insoluble proteins may be validated by separating the proteins of each fraction (supernatant: soluble proteins; pellet: insoluble proteins) by SDS-PAGE, as shown in Fig. 2C. 
- Requirement for concentration: In principle, lysates may not always need to be concentrated prior to calibration, but in practice it is recommended to ensure that there is a high enough concentration in the first few dilutions to get accurate protein concentration measurements from the absorbance readings. The total volume of lysate required may in some cases require trial and error, but 1.6ml (equivalent of 16 OD cells) is a good starting point. If 40 OD cells were lysed, up to 4ml lysate can be concentrated at this step. Another good rule of thumb (for green and red FPs at least) is that the FP stock should be concentrated enough to produce visibly colourful solutions.

Protein assay

- Typical raw data traces from absorbance spectra are provided in Supplementary Fig. 6A. Note the absorbance in the 900-1000nm range used for path length calculation, and the FP-specific absorbance in the intermediate wavelengths. Raw spectra that include wavelengths below 300nm will also contain a characteristic overflow absorbance in the UV range (most plastic microplates absorb in the UV range).
- If the peak is not evident by eye, this can indicate a low starting concentration of protein. After normalisation these usually become apparent, but if they do not, a higher starting concentration of protein is needed.

Fluorescence assay

- Visual inspection of raw fluorescence data can usually determine whether the dilutions are reasonably accurate and the replicates reasonably uniform.


