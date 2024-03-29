# Knowledge_transfer_with_Tanimoto_similarity

The code in this repository supports the thesis by Wang Wei How Marcus titled "Machine learning in predictive toxicology: investigating developmental and reproductive toxicity with transfer learning"

Code for chapter 3 of the thesis by Wang Wei How Marcus - Knowledge transfer between different human targets in predictive toxcicology using Tanimoto similarity and machine learning

Acknowledgement of the authors and the thesis is appreciated either when using the code partially or in full.

The Python 3 code for this project is available for download. The "Knowledge transfer" notebook contains the following code for:

 - Fingerprint generator
 - Modeller
 - For calculating similarities of specified targets vs all 79 targets
 - For calculating similarities of specified targets vs all 79 targets (with Multiprocessing)
 - For scrubbing datasets

The "Extraction and calculations for PubChem data" notebook contains the following code for:
 - Extracting and calculating similarities of PubChem data vs all 79 targets

The "Extraction and calculations for ChEMBL data" notebook contains the following code for:
 - Extracting and calculating similarities of ChEMBL data vs all 79 targets

To run code, select the required cell(s)/code blocks in the notebook and run them.

The workflow calculates the proportion of molecules in a dataset that is above the specified Tanimoto threshold with the other dataset and with the same active state.
This is performed for the first dataset with the second dataset, and for the second dataset with the first dataset. The average similarity between datasets is defined as the 
average of these two values.

Fingerprint generator and Modeller code were taken from:
https://github.com/teha2/chemical_toxicology/tree/master/NeuralNetworks-March2020
T. E. H. Allen, A. J. Wedlake, E. Gelžinytė, C. Gong, J. M. Goodman, S. Gutsell and P. J. Russell, Chem. Sci., 2020, 11, 7335–7348.

Datasets used for this study were also taken from the above link/study.
https://github.com/teha2/chemical_toxicology/tree/master/NeuralNetworks-March2020/Comparison%20Data
T. E. H. Allen, A. J. Wedlake, E. Gelžinytė, C. Gong, J. M. Goodman, S. Gutsell and P. J. Russell, Chem. Sci., 2020, 11, 7335–7348.
