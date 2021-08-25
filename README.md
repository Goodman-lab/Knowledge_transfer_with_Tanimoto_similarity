# AD-transferability
Code for the paper - Quantifying Applicability Domain transferability using Tanimoto similarity: A toxicological perspective

Acknoweldgement of the authors are required when using the code partially or in full.

The Python 3 notebook for this project is available for download. The notebook contains the following code for:

 - Fingerprint generator
 - Modeller
 - For calculating similarities of specified targets vs all 79 targets
 - For calculating similarities of specified targets vs all 79 targets (with Multiprocessing)
 - For scrubbing datasets
 - Extracting and calculating similarities of PubChem data vs all 79 targets
 - Extracting and calculating similarities of ChEMBL data vs all 79 targets

To run code, select the required cell(s)/code blocks in the notebook and run them.

The similarity indicator calculates the proportion of molecules in a dataset that is above the specified Tanimoto threshold with the other dataset and with the same active state.
This is performed for the first dataset with the second dataset, and for the second dataset with the first dataset. The average similarity indicator takes the average of these two
values.

Fingerprint generator and Modeller code were taken from:
https://github.com/teha2/chemical_toxicology/tree/master/NeuralNetworks-March2020
T. E. H. Allen, A. J. Wedlake, E. Gelžinytė, C. Gong, J. M. Goodman, S. Gutsell and P. J. Russell, Chem. Sci., 2020, 11, 7335–7348.

Datasets used for this study were also taken from the above link/study.
https://github.com/teha2/chemical_toxicology/tree/master/NeuralNetworks-March2020/Comparison%20Data
T. E. H. Allen, A. J. Wedlake, E. Gelžinytė, C. Gong, J. M. Goodman, S. Gutsell and P. J. Russell, Chem. Sci., 2020, 11, 7335–7348.
