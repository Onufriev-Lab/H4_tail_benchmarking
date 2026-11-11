# H4tailSAXSMDAnalyzer

<img width="6015" height="2523" alt="H4SAXSMDgraphic" src="https://github.com/user-attachments/assets/4f9d8087-85f7-451c-98fb-393d7e97f9df" />

**Overview** <br />
Repository containing tools to compare intrinsically disordered protein structural ensembles generated from molecular dynamics with small-angle X-ray scattering (SAXS) data. <br />
An example case is provided of the H4 histone tail, as part of the paper below. If you happen to use the code in this repository, please cite this paper. <br />
**Tong Wang^, Egor S. Kolesnikov^, Lois Pollack, Alexey V. Onufriev. Combining atomistic simulation and solution scattering to reveal charge-driven histone H4 tail conformational changes. (2026, in submission)** <br />

**Contents** <br /> 
To calculate SAXS profiles from SAXS data, please consult the ATSAS manual, specifically GAJOE, which uses CRYSOL: https://www.embl-hamburg.de/biosaxs/manuals/atsas-2.4/eom.html <br /> 
Experimental SAXS profiles for wild type and K-to-Q (charge neutralized) H4 histone tail are provided in the folder SAXSData <br />
Once GAJOE results are generated, you may run make2Dplot_fromEOMresults.m to generate a 2D histogram comparing a full MD ensemble with a SAXS-refined ensemble, as well as calculate the Jensen-Shannon divergence between the two distributions. <br />
The folder ExampleData contains an example GAJOE results output folder. 

**Hardware Notes** <br />
The analysis should only require a standard computer that is able to run the commonly available software below, with enough memory to complete moderate intensity computing tasks. <br />

**Software Notes** <br />
Molecular dynamics simulations are run using __ <br />
MATLAB R2021 or later may be required <br />

**License** <br />
This project is covered under the Apache 2.0 License.
