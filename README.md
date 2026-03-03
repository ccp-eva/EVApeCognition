 # <img src="https://github.com/user-attachments/assets/cee0bb16-3166-4109-b489-e646159b40c3" alt="Logo-EVApeCognition" width="30"> EVApeCognition Dataset
[![DOI](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.18847000-blue)](https://doi.org/10.5281/zenodo.18847000)

The **EVApeCognition Dataset** is an open-access collection of datasets from published great ape cognition studies located in https://doi.org/10.5281/zenodo.18846348. All studies included in the EVApeCognition Dataset were conducted at the Wolfgang Köhler Primate Research Center (WKPRC) located at Leipzig Zoo (Germany). The EVApeCognition Dataset is supported by the  **Max Planck Society for the advancement of Science**. 

The EVApeCognition Dataset is organized by publication. Each publication folder is given a unique identification comprised of the last name of the first author, the year of publication, and the first word in the title of the publication. 

Each publication folder included in the EVApeCognition Dataset contains the following files:
  - A metadata file (file contents listed below; .yaml) 
  - Full reference
  - Author list
  - The published abstract
  - Cognitive domain (social or physical), general domain, and specific domain  
  - Metadata for each of the experiments within the publication
  - Standardized data file(s) in (.csv) per experiment within the publication
  - A glossary indicating the description of each variable in the corresponding standardized data file(s) (.csv) per experiment within the publication

In addition to the study-specific files in each publication folder, the repository also contains general files that pertain to the dataset as a whole and provide relevant context. These files are as follows:
  - A csv file with general information about the great apes at the WKPRC (.csv) provided by staff at the WKPRC. 
  - A csv file with a list of contributed studies. This file includes reference information and the abstract. 
  - A csv file with a list of experiments within contributed studies. This file clarifies which experiments have available data, drop out information, group_ids of participants, and information regarding date of data collection and age of participants.
  - A csv file including definitions for group_ids,  such as location of research institution and participant species.
  - A csv file which includes information regarding the domains explored within the list of contributed studies
  - README file with information on dataset usage.

To facilitate navigation of the EVApeCognition Dataset, feel free to use the EVApeCognition.db file located in the general_files/SQLite_database/ folder. This was created using SQLite (Hipp, 2000)

The EVApeCognition Dataset complies with the **FAIR Data Principles** (Wilkinson et al., 2016). The EVApeCognition is **open-access (CC-BY 4.0)**. 

We do not take responsibility for the accuracy or completeness of the data provided by corresponding authors in the EVApeCognition Dataset. The corresponding authors of the publications are responsible for the accuracy and completeness of the contributed data from their publications as they accepted the final version for each dataset contained in the EVApeCognition Dataset by the time of publication. UTF-8 encoding is used for both the data files and their respective glossaries. 

![Picture3](https://github.com/user-attachments/assets/2e1504be-2197-4979-9413-a094062ed067)
