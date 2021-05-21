# WHOM_Dissemination
Data from the paper "Dissemination dynamics of receding words: A diachronic case study of *whom*" (Bohmann, Bohmann &amp; Hinrichs)

This repository contains intermediate data created from the Corpus of Historical American English (pre-2021 version) for the paper "Dissemination dynamics of receding words: A diachronic case study of *whom*" (Bohmann, Bohmann &amp; Hinrichs; currently under revision for publication in *Frontiers of Artificial Intelligence*).

Each sub-folder holds data relevant for one of the four dissemination measures used in the paper:

* COHA_Ds: Social dissemination as defined in Altmann et al. (2011) and Altmann et al. (2013).
   * COHA_Freq_rel_rho.7z: contains the relative frequency of each word with a total corpus frequency of at least 1,000, separately for each year in the period covered by COHA (1810-2009). The last column is Spearman's rho for the word's correlation between year and relative frequency, i.e. its monotonic rise or fall over time.
   * COHA_200_textfreq.7z: contains all document frequencies for the 100 most strongly rising and the 100 most strongly declining words in COHA. This can be used to calculate the social dissemination measure.
* COHA_Dl: Linguistic dissemination as defined in Stewart & Eisenstein (2018).
   * LxD_trigrams_allyears_10k.7z: The yearly corpus frequencies and unique trigram counts for a random selection of 10,000 of the words occurring at least 1,000 times in COHA on the whole. For each year, the number of words is slightly below 10,000, as some terms do not occur. This can be used to caluculate the expected (log) trigram count and, on that basis, the linguistic dissemination measure.
* COHA_Dr: Register dissemination, a newly proposed measure in the paper.
   * COHA_MDA_feats_fiction.7z, COHA_MDA_feats_magazine.7z, COHA_MDA_feats_news.7z, COHA_MDA_feats_nonfiction.7z: Frequencies of the 179 features in each text that were used for the multi-dimensional analysis.
   * COHA_POS_trigrams: A list of all part-of-speech trigrams in COHA with their respective absolute counts.
   * StructureCoefs5.txt: The structure coefficients (often referred to as "loadings") of each of the 179 features in combination with each of the five dimensions of variation
   * PatternCoefs5.txt: The pattern coefficients (often referred to as "loadings") of each of the 179 features in combination with each of the five dimensions of variation (see Thompson 2004).
   * ScoreCoefsRegression5.txt: The coefficients used for scoring individual corpus texts on each of the five dimensions, based on the feature frequencies in the COHA_MDA_feats*.7z files.
* COHA_Dt: Topic dissemination, another newly proposed measure.
   * COHA_Topics_Top30_words.csv: The top 30 words in each of the 25 topics, along with their probabilities in that topic's probability distribution over all words.
   * COHA_Topics_per_File.csv: For each corpus document, the associated probability distribution over the 25 topics.

References:

Altmann, Eduardo G., Janet B. Pierrehumbert & Adilson E. Motter. 2011. Niche as a determinant of word fate in online groups. *PLOS ONE*. Public Library of Science 6(5). e19009. https://doi.org/10.1371/journal.pone.0019009.

Altmann, Eduardo G., Zakary L. Whichard & Adilson E. Motter. 2013. Identifying trends in word frequency dynamics. *Journal of Statistical Physics 151(1–2)*. 277–288. https://doi.org/10.1007/s10955-013-0699-7.

Stewart, Ian & Jacob Eisenstein. 2018. Making “fetch” happen: The influence of social and linguistic context on nonstandard word growth and decline. In *Proceedings of the 2018 Conference on Empirical Methods in Natural Language Processing*, 4360–4370. Brussels, Belgium: Association for Computational Linguistics. https://doi.org/10.18653/v1/D18-1467.

Thompson, Bruce. 2004. *Exploratory and Confirmatory Factor Analysis: Understanding Concepts and Applications*. Washington, DC: American Psychological Association.
