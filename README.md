# Generalized Regression Neural Network Ensemble For Single Imputation

#### Project Status: [Active]  

## Objective  
The purpose of this project is to impute the missing data in numerical as well as categorical datasets.  

### Methods Used  
* SAGA (Simulated Annealing Genetic Algorithm) for Feature Selection  
* Generalized Regression Neural Network (GRNN) for Model Building  
* K-Fold Cross Validation for Data Validation  

### Technologies Used  
* Python (tqdm, pandas, numpy, seaborn, scipy, scikit-learn)  

## Project Description
* The project deals with development of Python code for single imputation of missing data using a generalized regression neural network for an unlabelled numerical and categorical dataset.  
* The incomplete data set will be divided into a complete and incomplete dataset. SAGA algorithm will be applied to choose the optimal subsets.  
* The subsets shall be used to train the GRNN, and the model will be fed to impute the missing data. Further we will calculate the NRMS (Normalized Root mean Square) value for numerical datasets and AE value for categorical dataset by comparing the imputed data sets with the original data sets.  
* Moreover, the algorithm shall be analyzed for runtime against the data size and dimensions.   

## Findings
* This pipeline achieved almost perfect results for all types of datasets given in the project achieving almost 0 Normalized Mean Squared Error and almost 98% accuracy.  
* As there were 26 datasets, which are large in number, it is difficult for an algorithm to work efficiently on all or most of them. Every dataset has different nature and flavor to it, feature selection techniques, algorithm to be chosen, and other elements in the analysis need to be very specific and fine tuned for optimum quality.  
* The Sonar dataset has the least percentage of missing data (20%) and letter dataset had the highest percentage of missing data (80%).  
* HOV is the fastest data that was computed in 13.78 seconds whereas the letter dataset took 2.75 hours to execute.  
