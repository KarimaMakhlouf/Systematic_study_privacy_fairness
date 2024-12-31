# Systematic_study_privacy_fairness
A Systematic and Formal Study of the Impact of Local Differential Privacy on Fairness.

Repository for the paper: A systematic and formal study of the impact of local differential privacy on fairness: Preliminary results [link to the paper](https://ieeexplore.ieee.org/abstract/document/10664426). 

# Codes & Datasets
All the experiments are implemented in Python 3. We use the Random Forest model for classification with its default hyper-parameters and randomly select 80% as the training set and
the remaining 20% as the testing set. For the RR mechanism, we use the implementation in [Multi-Freq-LDPy Python library](https://github.com/hharcolezi/multi-freq-ldpy). Since LDP protocols and ML algorithms are randomized, we report average results over 100 runs. 
* The [datasets](https://github.com/KarimaMakhlouf/Systematic_study_privacy_fairness/tree/main/Datasets) folder includes all the used and generated datasets. In total, six synthetic datasets and four real-world datasets are used to validate our results.
* The [Results](https://github.com/KarimaMakhlouf/Systematic_study_privacy_fairness/tree/main/Results) folder contains all the results (as csv files) of fairness metrics before and after applying the RR mechanism settings for all the datasets. 
  
* For each dataset, three Jupyter notebooks are available:
    - 1_Generated_data.ipynb: Jupyter notebook for generating (for the synthetic dataset) or preprocessing (for the Adult and Compas datasets) the data.
    - 2_Experiments.ipynb: Jupyter notebook for computing fairness metrics and accuracy before and after applying KRR mechanism settings.
    - 3_Generating_Plots.ipynb: Jupyter notebook for generating all the paper results.
    
# Environment
Our codes were developed using Python 3 with numpy, and pandas libraries. The versions are listed below:
* Python 3.7.3
* Numpy 1.21.2
* Pandas 1.3.3
* Multi-freq-ldpy 0.2.4

# On-going
The repository is still under cleaning/generalization of the codes and the documentation.

# Merits
* We use the randomized mechanism *RR* implemented in the [multi-freq-ldpy](https://github.com/hharcolezi/multi-freq-ldpy) library.
* We use the *Adult* dataset from the [folktables](https://github.com/socialfoundations/folktables) library.
* We use the *Compas* dataset from the [Kaggle](https://www.kaggle.com/datasets/danofer/compass) repository.
* We use the *German credit* dataset from the [folktables](https://archive-beta.ics.uci.edu/ml/datasets/statlog+german+credit+data) library.
* We use the *LSAC* dataset from the [Kaggle](https://eric.ed.gov/?id=ED469370) repository.


# Contact
For any questions, please contact:
[Karima Makhouf](http://www.lix.polytechnique.fr/Labo/Karima.MAKHLOUF/): karima.makhlouf [at]lix.polytechnique.fr


