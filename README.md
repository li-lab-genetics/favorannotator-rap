# favorannotator (DNAnexus Platform App)

This is the source code for the favorannotator app that runs on the DNAnexus Platform.
For more information about how to run or modify it, see
https://documentation.dnanexus.com/.

### Applet Usage
The **favorannotator** app is designed to functionally annotate genotype data in Genomic Data Structure (GDS) format of any genetic study using the <a href="https://doi.org/10.7910/DVN/1VGTJI">FAVOR Database</a> and create an annotated GDS (AGDS) file by storing the genotype data and their functional annotation data in an all-in-one file. The AGDS file can then facilitate a wide range of functionally-informed downstream analyses, for example, phenotype-genotype association analyses using the <a href="https://github.com/xihaoli/staarpipeline-rap">**staarpipeline**</a> app.

Please see the <a href="https://tinyurl.com/staarpipeline">**user manual and tutorial**</a> for detailed usage of favorannotator app.

### Cloning an Applet
To acquire the favorannotator applet, you will need to compile this applet for your respective DNANexus project, by cloning the repository from github and `dx build` an APPLET into your own workspace.

1. Clone this github repo to some directory:

```commandline
git clone https://github.com/xihaoli/favorannotator-rap.git
```

This will create a folder named favorannotator-rap, you can then:

2. Compile the source code:

```commandline
dx build -f favorannotator-rap
```

the `-f` flag just tells DNANexus to overwrite older versions of the applet within the same project if it is already there.

You can then run the following to run this applet:

```commandline
dx run favorannotator-rap <options>
```

### Citation
Zilin Li*, Xihao Li*, Hufeng Zhou, Sheila M. Gaynor, Margaret S. Selvaraj, Theodore Arapoglou, Corbin Quick, Yaowu Liu, Han Chen, Ryan Sun, Rounak Dey, Donna K. Arnett, Lawrence F. Bielak, Joshua C. Bis, Thomas W. Blackwell, John Blangero, Eric Boerwinkle, Donald W. Bowden, Jennifer A. Brody, Brian E. Cade, Matthew P. Conomos, Adolfo Correa, L. Adrienne Cupples, Joanne E. Curran, Paul S. de Vries, Ravindranath Duggirala, Barry I. Freedman, Harald H. H. Göring, Xiuqing Guo, Rita R. Kalyani, Charles Kooperberg, Brian G. Kral, Leslie A. Lange, Ani Manichaikul, Lisa W. Martin, Braxton D. Mitchell, May E. Montasser, Alanna C. Morrison, Take Naseri, Jeffrey R. O’Connell, Nicholette D. Palmer, Patricia A. Peyser, Bruce M. Psaty, Laura M. Raffield, Susan Redline, Alexander P. Reiner, Muagututi‘a Sefuiva Reupena, Kenneth M. Rice, Stephen S. Rich, Jennifer A. Smith, Kent D. Taylor, Ramachandran S. Vasan, Daniel E. Weeks, James G. Wilson, Lisa R. Yanek, Wei Zhao, NHLBI Trans-Omics for Precision Medicine (TOPMed) Consortium, TOPMed Lipids Working Group, Jerome I. Rotter, Cristen J. Willer, Pradeep Natarajan, Gina M. Peloso and Xihong Lin. (2021). **A framework for detecting noncoding rare variant associations of large-scale whole-genome sequencing studies**. _bioRxiv_. DOI: <a href="https://doi.org/10.1101/2021.11.05.467531">10.1101/2021.11.05.467531</a>.

Xihao Li*, Zilin Li*, Hufeng Zhou, Sheila M. Gaynor, Yaowu Liu, Han Chen, Ryan Sun, Rounak Dey, Donna K. Arnett, Stella Aslibekyan, Christie M. Ballantyne, Lawrence F. Bielak, John Blangero, Eric Boerwinkle, Donald W. Bowden, Jai G. Broome, Matthew P. Conomos, Adolfo Correa, L. Adrienne Cupples, Joanne E. Curran, Barry I. Freedman, Xiuqing Guo, George Hindy, Marguerite R. Irvin, Sharon L. R. Kardia, Sekar Kathiresan, Alyna T. Khan, Charles L. Kooperberg, Cathy C. Laurie, X. Shirley Liu, Michael C. Mahaney, Ani W. Manichaikul, Lisa W. Martin, Rasika A. Mathias, Stephen T. McGarvey, Braxton D. Mitchell, May E. Montasser, Jill E. Moore, Alanna C. Morrison, Jeffrey R. O'Connell, Nicholette D. Palmer, Akhil Pampana, Juan M. Peralta, Patricia A. Peyser, Bruce M. Psaty, Susan Redline, Kenneth M. Rice, Stephen S. Rich, Jennifer A. Smith, Hemant K. Tiwari, Michael Y. Tsai, Ramachandran S. Vasan, Fei Fei Wang, Daniel E. Weeks, Zhiping Weng, James G. Wilson, Lisa R. Yanek, NHLBI Trans-Omics for Precision Medicine (TOPMed) Consortium, TOPMed Lipids Working Group, Benjamin M. Neale, Shamil R. Sunyaev, Gonçalo R. Abecasis, Jerome I. Rotter, Cristen J. Willer, Gina M. Peloso, Pradeep Natarajan, & Xihong Lin. (2020). **Dynamic incorporation of multiple in silico functional annotations empowers rare variant association analysis of large whole-genome sequencing studies at scale**. _Nature Genetics_, _52_(9), 969-983. PMID: <a href="https://www.ncbi.nlm.nih.gov/pubmed/32839606">32839606</a>. PMCID: <a href="https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7483769/">PMC7483769</a>. DOI: <a href="https://doi.org/10.1038/s41588-020-0676-4">10.1038/s41588-020-0676-4</a>.
