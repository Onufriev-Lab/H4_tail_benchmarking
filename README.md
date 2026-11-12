# IDP MD-SAXS benchmarking

<img width="6112" height="2812" alt="H4SAXSMDgraphic" src="https://github.com/user-attachments/assets/328c5a72-924c-43e9-93a6-d43f74d66d93" />

**Overview** <br />
Repository containing tools to compare intrinsically disordered protein (IDP) structural ensembles generated from molecular dynamics (MD) with small-angle X-ray scattering (SAXS) data. <br />
An example case is provided of the H4 histone tail, as part of the paper below. If you happen to use the code in this repository, please cite this paper. <br />
**Tong Wang^, Egor S. Kolesnikov^, Lois Pollack, Alexey V. Onufriev. Combining atomistic simulation and solution scattering to reveal charge-driven histone H4 tail conformational changes. (2026, in submission)** <br />

**Contents** <br /> 
Regarding the ensemble optimization method (EOM): To calculate SAXS profiles from SAXS data, please consult the ATSAS manual, specifically GAJOE, which uses CRYSOL: https://www.embl-hamburg.de/biosaxs/manuals/atsas-2.4/eom.html <br /> 
The folder ExampleData contains an example GAJOE results output folder. <br />
Experimental SAXS profiles for wild type and K-to-Q (charge neutralized) H4 histone tail are provided in the folder SAXSData. <br />

Once GAJOE results are generated, you may run make2Dplot_fromEOMresults.m to generate a 2D histogram comparing a full MD ensemble with a SAXS-refined ensemble, as well as calculate the Jensen-Shannon divergence between the two distributions. <br />
You may also run plotEOMSAXScomparison.m to generate an averaged SAXS profile from an EOM/GAJOE result and plot and compare to experimental data. <br /> 
Both of these scripts are run by interacting with the "User-defined parameters" in the first code block. Mostly the paths just need to be matched. <br /> 

**Hardware Notes** <br />
The analysis should only require a standard computer that is able to run the commonly available software below, with enough memory to complete moderate intensity computing tasks. <br />

**Software Notes** <br />
EOM and GAJOE require the ATSAS SAXS modelling software. Using GAJOE v2.1 will be easiest. <br />
Molecular dynamics simulations are run using AMBER 24 <br />
MATLAB R2021 or later may be required <br />

**License** <br />
This project is covered under the Apache 2.0 License.
