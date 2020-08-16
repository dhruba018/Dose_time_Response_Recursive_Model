### Dose_time_Response_Recursive_Model  
Majority of the drug sensitivity prediction models attempt to predict a single representative metric of the complete dose-response curve such as IC<sub>50</sub> or AUC. This can potentially fail to provide some crucial information such as the trend of change in sensitivity as dose increases or the difference in sensitivity trends between two dose-response curves with similar AUC and/or IC<sub>50</sub> values. These information can often be used for a particular patient receiving precision therapy to select the most effective drug dosage or to avoid potential drug toxicity at the current time point. Here we develop a recursive methodology to model the complete dose-time drug response profile post drug administration that follows [Gompertz law](https://en.wikipedia.org/wiki/Gompertz%E2%80%93Makeham_law_of_mortality) in time and [sigmoidal model](https://en.wikipedia.org/wiki/Sigmoid_function) in dose, and can be used to predict the sensitivity at a certain dose and/or time. 

The details of the model is described in this 2019 paper: [Recursive model for dose-time responses in pharmacological studies](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-019-2831-4). This repository contains the necessary code to reproduce the results described in the paper and the corresponding data for the synthetic experiment.  

**Description.**  
The file 'RecursiveHybridModel.m' contains the model class with all necessary functions. The synthetic data example is provided in the file 'synthetic_recursive.mat' and the corresponding simulation code is provided in 'synthetic_data_analysis_SRD_v2.m'. 
