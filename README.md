# Protein Sequence-to-Structure Prediction

MNNN (Multi-scale Neighborhood-based Neural Network) is an example code for predicting dihedral angles using only primary protein sequences. It is useful for computing  3D structural information of known and unknown protein sequence. 

![image](https://user-images.githubusercontent.com/101393859/235613396-8c28a6d3-d6fa-4842-9255-2619f5a7ad0b.png)

Abstract: The development of rational techniques to discover new mechanically relevant proteins for use in variety of applications ranging from mechanics, agriculture to biotechnology remains an outstanding nanomechanical design problem. The key barrier is to design a sequence to fold into a predictable structure to achieve a certain material function. Focused on alpha-helical proteins (as found in skin, hair, and many other mechanically relevant protein materials), we report a Multi-scale Neighborhood-based Neural Network (MNNN) model to learn how a specific amino acid sequence folds into a protein structure. The algorithm predicts the protein structure without using a template or co-evolutional information at a maximum error of 2.1 Å. We find that the prediction accuracy is higher than other models and the prediction consumes less than six orders of magnitude time than ab initio folding methods. We demonstrate that MNNN can predict the structure of an unknown protein that agrees with experiments, and our model hence shows a great advantage in the rational design of de novo proteins.

Publication: Z. Qin, L. Wu, H. Sun, S. Huo, T. Ma, E. Lim, P.-Y. Chen, B. Marelli, M.J. Buehler, Artificial intelligence method to design and fold alpha-helical structural proteins from the primary amino acid sequence, Extreme Mechanics Letters, Vol. 36, 100652, 2020. https://doi.org/10.1016/j.eml.2020.100652.

Dataset: https://doi.org/10.5281/zenodo.7885535 

## Requisites

python>=3.6.

tensorflow==1.8.

sklearn==0.19.1 

matplotlib==2.0.2

## How to train the model:

python MNNN/food_train.py

## Inference/tesing:

(1) paste target data into MNNN/foodData/testData.txt. (format: "ABC... %name", as example)

(2) run MNNN/foodData/interGen.py to reformat the input data.

(3) run MNNN/inferrence.py to get model output.

(4) run MNNN/generateOutput.py to reformat output data based on configurations.

(5) run MNNN/results/npyRes/printPreds.py to display the output model predictions, output path: MNNN/results/npyRes/output.txt  
