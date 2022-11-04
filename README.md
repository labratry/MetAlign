# MetAlign
This repository contains the source and documentation of the MetAlign suite published by Dr. Ir. Arjen Lommen in November 2, 2022 on [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7273832.svg)](https://doi.org/10.5281/zenodo.7273832) 
licenced under the [Creative Commons Attribution Non Commercial Share Alike 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/legalcode).

We like to invite everyone to participate in the software by [reporting issues](https://github.com/labratry/MetAlign/issues) improving the code with [pull requests](https://github.com/labratry/MetAlign/pulls) 
and sharing ideas or questions in [the discussions}(https://github.com/labratry/MetAlign/discussions/).

## General introduction and personal note from the original author
Dr. Ir. Arjen Lommen has dedicated the most part of his 37-year scientific work to data analysis. In the second half of the 80’s  he started automating data analysis on an IBM mainframe using APL. After 1990 he taught himself to write programs in C on a SUN Unix machine to be able to process the 3rd dimension in 3D-NMR analysis. With no chemometric experience and only a slight background in IT, this continued into writing programs to extract and align signals from 1D-NMR data. Algorithms were not based on chemometrics, but derived from how a trained person would analyse data visually or by hand. Eventually the NMR software transformed after 1998 into software for low resolution GCMS and then to low resolution LCMS using Microsoft Visual C++ and personal computers. This then went on to automation of low resolution GCGCMS. After 2009 the developments went further towards high-resolution GCMS and LCMS with the emphasis on Orbitrap-MS. Now in 2022 the evolution of this software due to the retirement of Arjen Lommen has come to an end.
Those who want to pick up on this should read the “Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International Public License” under which the software is available free of charge. They should also realize that the software was not written by an IT-expert or a chemometrics expert, but by someone who taught himself.
The general way the software was structured was through an interface that runs multiple separate and consecutive programs in a batch format under Windows (compatible at least until Windows 10). All software has been thoroughly debugged, but software is never finished and always needs some update once in a while.

### Description and key publications
The MetAlign suite is now available including source code (Microsoft Visual C++ 2010) under the “Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International Public License”.
The suite of software was last used internationally for data analysis in the SPECIMEn (Survey on PestiCIde Mixtures in Europe) within HBM4EU (Human Biomonitoring for Europe) [1-3]. Within WFSR it is still actively used for data analysis related to statutory tasks.
The software (incl Windows Visual C++ source code) shared here comprises:
1. Metalign : Data preprocessing and alignment [4,5].
2. HR_MS_search : Ultra-fast searching module for searching large numbers of metAlign-preprocessed data files with templates. It includes software for RT and mass corrections such as performed in the SPECIMEn study. [6-8]
3. Extract_lcms : Automated adduct and elemental composition analysis of metAlign pre-processed full scan Orbitrap-MS data. Annotation based on a csv template and secondly based on a ultra-fast pubchem search. Mining program for sophisticated annotation present. [7]
4. HR3 : Standalone program for elemental composition analysis with modified 7 golden rules (can use ultrafast pubchem format (see below)) [7]
5. Checkconvert_csv_file : Program to create a search template for HR_MS_search starting from molecular formulas in an annotation template.
6. Make_pubchem_lib : Conversion of Pubchem format to ultra-fast pubchem search format for Extract_LCMS and HR3 [7]
7. Redms_converter : Program to change metAlign-preprocessed format (redms_acc) back to Masslynx or Xcalibur format.
8. metAlignID: Originally software for mining LECO GCGCMS data (LECO format may have changed meanwhile). Now the search_GCMS module is used for matching subspectra to libary spectra. A program to make NIST-type libraries compatible is present. [9]
9. Change_calibration_work: program with which databases of redms_acc files or search_template csvs can be recalibrated (for instance RT) to fit a different LC-MS.

### Relevant publications
1. Huber et al, Environment International, Volume 168, October 2022, 107452. A large scale multi-laboratory suspect screening of pesticide metabolites in human biomonitoring: From tentative annotations to verified occurrences.
2. Vitale et al, Anal. Chem. 2022, 94, 22, 7833–7843. Harmonized Quality Assurance/Quality Control Provisions for Nontargeted Measurement of Urinary Pesticide Biomarkers in the HBM4EU Multisite SPECIMEn Study.
3. De Vos et al, Nature Protocols volume 2, pages 778–791 (2007). Untargeted large-scale plant metabolomics using liquid chromatography coupled to mass spectrometry.
4. Lommen, Anal. Chem., 81 (8) (2009), pp. 3079-3086. MetAlign: Interface-Driven, Versatile Metabolomics Tool for Hyphenated Full-Scan Mass Spectrometry Data Preprocessing.
5. Lommen & Kools, Metabolomics, 8 (4) (2012), pp. 719-726. MetAlign 3.0: Performance Enhancement by Efficient Use of Advances in Computer Hardware.
6. Lommen et al, Metabolomics, 7 (1) (2011), pp. 15-24. Ultra-Fast Searching Assists in Evaluating Sub-Ppm Mass Accuracy Enhancement in U-HPLC/Orbitrap MS Data.
7. Lommen, Anal. Chem., 86 (11) (2014), pp. 5463-5469. Ultrafast PubChem Searching Combined with Improved Filtering Rules for Elemental Composition Analysis.
8. Lommen et al, Rapid Commun. Mass Spectrom., 33 (20) (2019), pp. 1578-1588. Ultra-Fast Retroactive Processing of Liquid Chromatography High-Resolution Full-Scan Orbitrap Mass Spectrometry Data in Anti-Doping Screening of Human Urine.
9. Lommen et al. Journal of Chromatography A, Volume 1263, 9 November 2012, Pages 169-178. metAlignID: A high-throughput software tool set for automated detection of trace level contaminants in comprehensive LECO two-dimensional gas chromatography time-of-flight mass spectrometry data

[Citation indices](https://scholar.google.com/citations?user=sgCwmUYAAAAJ) of Arjen Lommen