# Resources for Students

_Created in 2017. Will be updated/overhauled over the coming months._

Here are a list of online resources (or lab ones) that should help you find information about sequences / molecular biology questions or basic protocols, and to help you troubleshoot your own experiments. Generally, resources are free and online. This list isn’t meant to be exhaustive, it is mainly to get you started.

---

### General Reference/Tools

* Bionumbers - https://bionumbers.hms.harvard.edu/search.aspx
* Calculators - conversions http://www.genscript.com/conversion.html
* PCR calculator - https://ec363.shinyapps.io/pcr_calc/

---

### MolBio Reference

**Codes and abbreviations**

* Nucleotide abbreviations - https://en.wikipedia.org/wiki/Nucleotide#Abbreviation_codes_for_degenerate_bases
  * DNA modifications (IDT) https://eu.idtdna.com/site/Catalog/Modifications/ 
* Modified dNTPs (and similar) - https://www.jenabioscience.com/nucleotides-nucleosides/nucleotides-by-structure
* Amino acid abbreviations - https://en.wikipedia.org/wiki/Proteinogenic_amino_acid#Chemical_properties
* Codon Table - https://en.wikipedia.org/wiki/DNA_codon_table . 

**Codon usage tables**

* E coli and others
  * http://www.kazusa.or.jp/codon/cgi-bin/showcodon.cgi?species=83333
  * http://openwetware.org/wiki/Escherichia_coli/Codon_usage
  * http://www.genscript.com/cgi-bin/tools/codon_freq_table

**Tools**

* Clustal Omega, DNA/RNA/Protein alignment http://www.ebi.ac.uk/Tools/msa/clustalo/
* Blast, sequence search in databases http://blast.ncbi.nlm.nih.gov/Blast.cgi?
* Back-translation http://www.ebi.ac.uk/Tools/st/

---

### General Lab Techniques

**Buffers**

* Buffer for biochemical reactions - 
  * https://www.promega.co.uk/resources/product-guides-and-selectors/protocols-and-applications-guide/buffers-for-biochemical-reactions/
  * http://www.sigmaaldrich.com/life-science/core-bioreagents/biological-buffers/learning-center/buffer-reference-center.html
  * http://www.sigmaaldrich.com/life-science/core-bioreagents/biological-buffers/learning-center/buffer-calculator.html

**Protocol databases / FAQs**

* http://cshprotocols.cshlp.org/site/misc/subject.xhtml
* http://openwetware.org/wiki/Protocols - open source protocols
* https://www.researchgate.net/topics - Join to let you browse Q&As better.
* https://barricklab.org/twiki/bin/view/Lab/ProtocolList 

---

### Molecular Biology Techniques

**Manuals**

* Reagent-specific info can be found on the manufacturer’s website. 
* Very basic protocols [agar plates, cultures, transformation, minipreps, agarose gels]
  * https://www.addgene.org/protocols/
  * Kits: Minipreps, PCR purification, Gel extraction - manuals within the boxes.

**DNA separation**

* kb ladders: 1kb - https://www.neb.com/products/n3232-1-kb-dna-ladder
* low MW - https://www.neb.com/products/n3233-low-molecular-weight-dna-ladder

**Protein electrophoresis.**

* ladder: https://www.neb.com/products/p7712-color-prestained-protein-standard-broad-range-11-245-kda
* hall of shame: http://www.ruf.rice.edu/~bioslabs/studies/sds-page/sdsgoofs.html
* Tricine-SDS-PAGE for small proteins and peptides <30 kDa (especially if <15 kDa, as 15-30 can just about be resolved by standard glycine/Laemmli-SDS-PAGE). This paper is great resource not just for Tricine gels but also for hydrophobic proteins, membrane proteins, SDS, DTT/beta-merc reducing agents, etc. 2006 Schägger et al. Nat Protocols doi:10.1038/nprot.2006.4

---

### CLONING - DNA Construct Design

**Software:**

* Benchling (free) - Labbook and DNA analysis package. https://www.benchling.com/
* Snapgene (£££) - DNA analysis package. http://www.snapgene.com/support/tutorial_videos/introduction_to_snapgene/

**Plasmid vectors:**

Plasmid databases:

* commercial
    * https://www.neb.com/tools-and-resources/interactive-tools/dna-sequences-and-maps-tool
    * https://www.embl.de/pepcore/pepcore_services/strains_vectors/vectors/bacterial_expression_vectors/popup_bacterial_expression_vectors/
* donated https://www.addgene.org/browse/
* other https://dnasu.org/DNASU/Home.do , https://dnasu.org/DNASU/SearchOptions.do?tab=1

Plasmid Parts

* iGEM Registry databases and distributions: http://parts.igem.org/assembly/libraries.cgi.
* Plasmid Origins http://blog.addgene.org/plasmid-101-origin-of-replication
* Antibiotic resistance genes - Vector/plasmid database
* Antibiotic working stocks - https://www.addgene.org/mol-bio-reference/antibiotics/
     though Cam is often used at 34µg/ml final, slightly more than 25 µg/ml.
* Restriction enzymes - SnapGene, EnzymeX, NEB website

**E coli Strains:**

* NEB 10beta- https://www.neb.com/products/c3020-neb-10-beta-electrocompetent-e-coli
* NEB T7 express lysY/lacIq- https://www.neb.com/products/c3013-t7-express-lysyiq-competent-e-coli-high-efficiency
* BL21(DE3)- https://www.neb.com/products/c2527-bl21de3-competent-e-coli
* More strains: https://www.addgene.org/mol-bio-reference/strain-information/
* Common lab strains: https://blog.addgene.org/plasmids-101-common-lab-e-coli-strains

**Construct:**

* Plasmid features
  * Snapgene has built in version
  * https://www.addgene.org/tools/reference/plasmid-features/
* Common Epitope Tags - https://www.addgene.org/mol-bio-reference/#tags
* RBS calculators 
  * https://www.denovodna.com/software/
  * https://salislab.net/software/
  * http://wolfson.huji.ac.il/expression/vector/RibosomalBindingSites.html
  * Andersen promoters (set of constititive promoters from weak to strong): iGEM pages.

**Primer design:**

* Snapgene has Tm calculations that work OK.
* IDT is more thorough: https://eu.idtdna.com/calc/analyzer
* with formulae: http://www.genscript.com/cgi-bin/tools/primer_calculation

**Enzymes**
* Enzymes used in molecular biology: a useful guide https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2570007/


### CLONING - In practice

* Types of cloning https://www.addgene.org/mol-bio-reference/cloning/
* Traditional cloning (Type II restriction digest)
  * https://www.addgene.org/mol-bio-reference/cloning/#re
  * https://www.addgene.org/protocols/subcloning/
  * https://www.addgene.org/protocols/pcr-cloning/
* __Type IIS cloning combined with PCR cloning (= recommended as default)__
  * https://www.addgene.org/mol-bio-reference/cloning/#typeIIs
* Oligo cloning - https://www.addgene.org/plasmid-protocols/annealed-oligo-cloning/
* Gibson assembly (also recommended)
  * https://www.addgene.org/plasmid-protocols/gibson-assembly/
  * http://openwetware.org/wiki/Janet_B._Matsen:Guide_to_Gibson_Assembly
* SPLiCE (by Edo Gianni) - http://openwetware.org/wiki/SPLiCE

**General cloning protocols:**

* Very basic protocols [agar plates, cultures, transformation, minipreps, agarose gels]
  * https://www.addgene.org/protocols/
  * Kits: Minipreps, PCR purification, Gel extraction - manuals within the boxes.
* Restriction enzymes - https://www.neb.com/tools-and-resources/usage-guidelines/nebuffer-performance-chart-with-restriction-enzymes
* Ligation http://www.addgene.org/plasmid-protocols/dna-ligation/
* Electroporation - see wet-lab-protocols

**PCR protocols:**

* Q5 - https://www.neb.com/protocols/2012/08/30/pcr-using-q5-hot-start-high-fidelity-dna-polymerase-m0493
* Taq - https://international.neb.com/protocols/0001/01/01/taq-dna-polymerase-with-standard-taq-buffer-m0273
* PCR calculator - https://ec363.shinyapps.io/pcr_calc/

**Sequencing:**

* Follow instructions on provider's webpage about how to prepare samples. They often have stock primers for standard plasmids.

---

### MICROBIOLOGY

* Commandments of experimental microbiology (Barrick) https://barricklab.org/twiki/bin/view/Lab/StandardMicrobiologicalPractices
* OD600 calculator http://www.genomics.agilent.com/biocalculators/calcODBacterial.jsp

**E coli strains/genotypes:**

* list of strain genotypes and what the genotypes mean http://openwetware.org/wiki/Escherichia_coli/Nomenclature_%26_Abbreviations
* List of E coli strains, but no links: http://www.uniprot.org/taxonomy/83333

**E coli genome/genes:**

* EcoGene (when it was live it was great) http://www.ecogene.org/

**E coli general:**

* openwetware (protocols): http://openwetware.org/wiki/Escherichia_coli
* wiki: http://ecoliwiki.net/colipedia/index.php/Welcome_to_EcoliWiki
    * strains http://ecoliwiki.net/colipedia/index.php/Category:Strains
    * gene lists http://ecoliwiki.net/colipedia/index.php/Category:Gene_Lists
    * genomes: http://ecoliwiki.net/colipedia/index.php/Category:E._coli_genomes
    * DH10b
        * http://ecoliwiki.net/colipedia/index.php/DH10B
        * genome https://www.ncbi.nlm.nih.gov/nucleotide/NC_010473
        * ref http://ecoliwiki.net/colipedia/index.php/PMID:18245285
    * BL21 (DE3)
        * https://www.ncbi.nlm.nih.gov/nuccore/NC_012971
* EcoCyc: http://ecocyc.org/
    * literature-based curation of the K12-MG1655 genome
* Characteristics of the E. coli genome (Barrick) https://barricklab.org/twiki/bin/view/Lab/ReferenceEColiGenome


---

### PROTEIN EXPRESSION (E coli)

Troubleshooting:

* EMBL https://www.embl.de/pepcore/pepcore_services/protein_expression/ecoli/index.html
* RBSCalculators: https://salislab.net/software/


### PROTEIN ANALYSIS 

**Protein structure databases**

* UniProt http://www.uniprot.org/
* PDB (Europe) http://www.ebi.ac.uk/pdbe/
* RCSB http://www.rcsb.org/pdb/home/home.do (Research Collaboratory for Structural Bioinformatics, US) 
* Others (list) - https://en.wikipedia.org/wiki/Protein_structure_database
of interest:
  * Proteopedia: essentially a wikipedia for proteins.
  * ProtCID - Protein common interface database (for homologous proteins).

**Amino acid properties**

* http://www.sigmaaldrich.com/life-science/metabolomics/learning-center/amino-acid-reference-chart.html
* https://en.wikipedia.org/wiki/Amino_acid
* https://en.wikipedia.org/wiki/Proteinogenic_amino_acid#Chemical_properties

**Protein Properties**

* Protein properties, Expasy http://www.expasy.org/resources

**Protein families by structure**

* SCOP http://scop2.mrc-lmb.cam.ac.uk/
* CATH http://www.cathdb.info/search
* Pfam http://pfam.xfam.org/

---

### EXPERIMENTAL DESIGN

* Intro to experimental design (Barrick) https://barricklab.org/twiki/bin/view/Lab/IntroductionToExperimentalDesign
* How to prepare figures (not a bad set of guidelines) https://barricklab.org/twiki/bin/view/Lab/ProtocolsGraphGuide


