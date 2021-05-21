# WHOM_Dissemination
Data from the paper "Dissemination dynamics of receding words: A diachronic case study of *whom*" (Bohmann, Bohmann &amp; Hinrichs)

This repository contains intermediate data created from the Corpus of Historical American English (pre-2021 version) for the paper "Dissemination dynamics of receding words: A diachronic case study of *whom*" (Bohmann, Bohmann &amp; Hinrichs; currently under revision for publication in *Frontiers of Artificial Intelligence*).

Each sub-folder holds data relevant for one of the four dissemination measures used in the paper:

* COHA_Ds: Social dissemination as defined in Altmann et al. (2011) and Altmann et al. (2013).
   * COHA_Freq_rel_rho.csv: contains the relative frequency of each word with a total corpus frequency of at least 1,000, separately for each year in the period covered by COHA (1810-2009). The last column is Spearman's rho for the word's correlation between year and relative frequency, i.e. its monotonic rise or fall over time.
* COHA_Dl: Linguistic dissemination as defined in Stewart & Eisenstein (2018).
* COHA_Dr: Register dissemination, a newly proposed measure in the paper.
* COHA_Dt: Topic dissemination, another newly proposed measure.
