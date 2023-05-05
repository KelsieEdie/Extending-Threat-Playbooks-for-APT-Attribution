# Extending Threat Playbooks for Cyber Threat Intelligence: A Novel Approach for APT Attribution 
## Purpose
This github repository contains code used to perform research in the field of cyber attack attribution. This research was published in ISDFS 2023 (https://isdfs.org). The link for the paper will be published soon. 
## Abstract
As cyber attacks grow in complexity and frequency,
cyber threat intelligence (CTI) remains a priority objective for
defenders. A critical component of CTI at the strategic level of
defensive operations is attack attribution. Attributing an attack to
a threat group informs defenders on adversaries that are actively
engaging them and advances their ability respond. In this paper,
we propose a data analytic approach towards threat attribution
using adversary playbooks of tactics, techniques, and procedures
(TTPs). Specifically, our approach uses association rule mining
on a large real world CTI dataset to extend known threat TTP
playbooks with statistically probable TTPs the adversary may
deploy. The benefits are twofold. First, we offer a dataset of
learned TTP associations and extended threat playbooks. Second,
we show that we can attribute attacks using a weighted Jaccard
similarity with 96% accuracy.
## Contents
* TTP_AAG.ipynb - contains the python notebook used to create the activity groups and generate the stix bundle of the activity attack graph.
* TTP_Data.csv - final dataset compiled from both Categorized_Adversary_TTPs.csv and pyattck. 
* Categorized_Adversary_TTPs.csv - This dataset is compiled from various cyber attacks. It contains metadata on the attacks and includes a list of ATT&CK T-codes: https://github.com/tropChaud/Categorized-Adversary-TTPs
* AbstractRules.csv - a CSV file of the abstract rules extracted from the dataset after replacing all sub-techniques with their parent technique. 
* SpecificRules - a CSV file of the specific rules extracted from the dataset. These rules have a combination of both techniques and sub-techniques. 
## Bibtex Citation
```
@inproceedings{edie_mckee_attribution_2023,
  title={Extending Threat Playbooks for Cyber Threat Intelligence: A Novel Approach for APT Attribution},
  author={Edie, Kelsie and McKee, Cole and Duby, Adam},
  booktitle={2023 IEEE 11th International Symposium on Digital Forensics and Security (ISDFS)},
  year={2023},
  organization={IEEE}
}
```
