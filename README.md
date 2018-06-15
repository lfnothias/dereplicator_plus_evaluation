# dereplicator_plus_evaluation
This repository contains the data and script from the evaluation of Dereplicator+ on 5414 spectral library annotations from GNPS libraries

## INTRODUCTION

For the evaluation on the Insilico Peptidic Natural Products Dereplicator see:
https://bix-lab.ucsd.edu/display/Public/Insilico+Natural+Products+Dereplicator+Documentation

The workflow can be accessed here: https://gnps.ucsd.edu/ProteoSAFe/static/gnps-theoretical.jsp

Citation:
Hosein Mohimani, Alexey Gurevich, Alla Mikheenko, Neha Garg, Louis-Felix Nothias, Akihiro Ninomiya, Kentaro Takada, Pieter C. Dorrestein, Pavel A. Pevzner, Dereplication of Peptidic Natural Products Through Database Search of Mass Spectra, Nature Chemical Biology 13, 30--37 (2017) https://www.nature.com/articles/nchembio.2

## METHODS

See the corresponding GitHub for the evaluation script and data: https://github.com/lfnothias/dereplicator_plus_evaluation

The results of the 5414 dereplicator+ have been evaluated against 5414 annotations spectral library matches. 75% of these spectral hits are entries from the NIH-GNPS spectral library available here.
https://gnps.ucsd.edu/ProteoSAFe/libraries.jsp

Results showed that with a threshold score of 3 (1574 annotations), the dereplicator+ finds the correct candidate at the first position for 55.5 % of spectra.

With a threshold score of 5 (865 annotations), the correct candidate is found at the first position for 68.4 % of spectra, while for 30.7 % of the incorrect annotations the candidate was found to have a strong structural similarity (calculated using the tanimonoto score between the pubchem fingerprint > 0.7).

With a threshold score of 8 (364 annotations), the correct candidate is found at the first position for 78.5 % of spectra, while for 52.5 % of the incorrect annotations the candidate was found to have a strong structural similarity (calculated using the tanimonoto score between the pubchem fingerprint > 0.7).

Overall, the dereplicator+ scoring function (Figure 1-2) was found to more significant than the dereplicator score (Figure 3-4).
### Dereplicator+

Figure 1.
<img src="IMG/figure1.png"/>

Figure 2.
### Dereplicator
<img src="IMG/figure2.png"/>

Figure 3.
<img src="IMG/figure3.png"/>

### Dereplicator+ vs Dereplicator

Figure 4. Distribution of the score for the correct annotation in dereplicator+ and dereplicator
<img src="IMG/figure4.png"/>

