# PDDA-Machine-Learning-Competition-2020

## SPWLA PDDA’s 1st Petrophysical Data-Driven Analytics Contest -- Sonic Log Synthesis


### Sponsored by:
[SPWLA-PDDA](https://www.spwla.org/SPWLA/Chapters_SIGs/SIGs/PDDA/PDDA.aspx)

[SparkCognition](https://www.sparkcognition.com/?utm_medium=direct&utm_source=direct)

### Leaderboard
Root mean squared error(RMSE) is calculated from the DTC and DTS values of the hidden dataset.

![equation](https://github.com/pddasig/Machine-Learning-Competition-2020/blob/master/pictures/CodeCogsEqn.png)

| Rank | Team Name              | Submission1  | Submission2  | Submission3 | Best Solution | Notebook                                                                                                                                                         | Best     |
|:----:|------------------------|--------------|--------------|-------------|---------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------|
|   1  | SedStrat               | 15.77521     |              |             |               |                                                                                                                                                                  | 15.77521 |
|   2  | Curiosity              | 17.88773     | 15.96676     |             |               |                                                                                                                                                                  | 15.96676 |
|   3  | Diagenesis             | 16.58438     |              |             |               |                                                                                                                                                                  | 16.58438 |
|   4  | SubsurfaceIntelligence | 16.92818     |              |             |               |                                                                                                                                                                  | 16.92818 |
|   5  | TeamTriumphant         | 17.15541     |              |             |               |                                                                                                                                                                  | 17.15541 |
|   6  | TrashPandas            | 20.60043     | 17.27522     |             |               |                                                                                                                                                                  | 17.27522 |
|   7  | HoustonEnergyTeam      | 17.30373     |              |             |               |                                                                                                                                                                  | 17.30373 |
|   8  | DataDrivenPancakes     | 17.64751     |              |             |               |                                                                                                                                                                  | 17.64751 |
|   9  | PDDA                   | 17.92553     | *            | *           | Randomforest  | [Starter_Yu.ipyb](https://github.com/pddasig/Machine-Learning-Competition-2020/blob/master/Synthetic%20Sonic%20Log%20Generation%20Starter_Yu%202_27_2020.ipynb)  | 17.92553 |


### Background
Well logs are interpreted/processed to estimate the in-situ petrophysical and geomechanical properties, which is essential for subsurface characterization. Various types of logs exist, and each provides distinct information about subsurface properties. Certain well logs, like gamma ray (GR), resistivity, density, and neutron logs, are considered as “easy-to-acquire” conventional well logs that are run in most of the wells. Other well logs, like nuclear magnetic resonance, dielectric dispersion, elemental spectroscopy, and sometimes sonic logs, are only run in limited number of wells.

Sonic travel-time logs contain critical geomechanical information for subsurface characterization around the wellbore. Often, sonic logs are required to complete the well-seismic tie workflow or geomechanical properties prediction. When sonic logs are absent in a well or an interval, a common practice is to synthesize them based on its neighboring wells that have sonic logs. This is referred to as sonic log synthesis or pseudo sonic log generation. 

### Problem Statement
Compressional travel-time (DTC) and shear travel-time (DTS) logs are not acquired in all the wells drilled in a field due to financial or operational constraints. Under such circumstances, machine learning techniques can be used to predict DTC and DTS logs to improve subsurface characterization. The goal of the “SPWLA’s 1st Petrophysical Data-Driven Analytics Contest” is to develop data-driven models by processing “easy-to-acquire” conventional logs from Well #1, and use the data-driven models to generate synthetic compressional and shear travel-time logs (DTC and DTS, respectively) in Well #2. A robust data-driven model for the desired sonic-log synthesis will result in low prediction errors, which can be quantified in terms of Root Mean Squared Error(RMSE) by comparing the synthesized and the original DTC and DTS logs.

You are provided with two datasets: Well #1 dataset and Well #2 dataset. You need to build a generalizable data-driven models using Well #1 dataset. Following that, you will deploy the newly developed data-driven models on Well #2 dataset to synthesize DTS and DTC logs. The data-driven model should use feature sets derived from the following seven logs: Caliper, Neutron, Gamma Ray, Deep Resistivity, Medium Resistivity, Photo-electric factor and density. The data-driven model should synthesize two target logs: DTC and DTS logs.


### About us
[Petrophysical Data-Driven Analytics (PDDA)](https://www.spwla.org/SPWLA/Chapters_SIGs/SIGs/PDDA/PDDA.aspx), a special interest group under society of Petrophysicists and Well Log Analysts (SPWLA), is announcing its first machine learning contest in 2020!
The contest is open to all SPWLA members (including student members) or whoever are interested in machine learning applications in petrophysics. 

### Competition Timeline 
Start Date: March 1, 2020 

Team Registration Deadline: March 31, 2020 11:59 PM CST

Entry Deadline: April 30, 2020 11:59 PM CST

End Date (Final Submission of Code Deadline): May 7, 2020 11:59 PM CST


### Registration 
Please send your team name, team member, contact info, and affiliation to pdda_sig@spwla.org. The official competition website is https://github.com/pddasig/Machine-Learning-Competition-2020. 

### One account per participant
You cannot register from multiple accounts and therefore you cannot submit from multiple accounts.


### Team Limits
The maximum team size is 5.


### Submission 
Your submission needs to follow the same format as the ‘sample_submission.csv’ file provided on the competition website, the final ranking is based on the RMSE score of the hidden dataset. 

A blind test dataset from 20% of the hidden dataset is released for the your judgement, you may check your model performance based on this dataset as many times as you want. This dataset will be released after the registration deadline. 

Please note that the purpose of the released dataset is providing a validation tool to check the performance of your model. However, in the real application there would be no such data, since we will not have any access to the new well's data. Therefore please do not use the data to train your model. 

You may select up to 3 submissions for judging before the entry deadline, the highest score will be used for your rank. 
You must submit your runnable code in a Notebook/JupyterNotebook format before the end date, any code submission with sever bugs or results in a different number from the data entry will not be ranked or awarded. 

** Please make sure to use **"random_state"** or **"SEED"** for all the steps that involves randomization in your model, this will ensure the same result run by the judges.    


### Privacy Rules
Privately sharing code or data outside of teams is not permitted. It's okay to share code if made available to all participants on the competition Github repository.

You should NOT use any dataset during the training other than the one provided by the committee.

Any violation of the above will be regarded as cheating and not ranked or awarded. 


### COMPETITION-SPECIFIC TERMS 
COMPETITION TITLE: Pseudo Sonic Log Generation 

COMPETITION ORGANIZOR: SPWLA – PDDA SIG

COMPETITION WEBSITE: https://github.com/pddasig/Machine-Learning-Competition-2020 

You can submit "Issues" ticket to the repository if you find any problem of the compeition or would like to raise a discussion topic. 


### PRIZES POLICY: 
Prize pool: __$1500__

Top 5 winning teams will be awarded with prizes(NOT in cash) based on the final prize pool.

Novel and practical algorithms will be recommended for a submission to the next SPWLA special issue by PDDA. 

### DATA LICENSING
The data comes from VOLVE dataset owned by Equinor. 

DATA ACCESS AND USE: Creative Commons Attribution-NonCommercial-ShareAlike license.

ENTRY IN THIS COMPETITION CONSTITUTES YOUR ACCEPTANCE OF THESE OFFICIAL COMPETITION RULES.

The Competition named above is a skills-based competition to promote and further the field of data science. You must submit your registration to pdda_sig@spwla.org to enter. Your competition submissions ("Submissions") must conform to the requirements stated on the Competition Website. Your Submissions will be scored based on the evaluation metric described on the Competition Website. Subject to compliance with the Competition Rules, Prizes, if any, will be awarded to participants with the best scores, based on the merits of the data science models submitted. Check the competition website for the complete Competition Rules.



### SPWLA PDDA SIG Contest Committee:
Yanxiang Yu, Michael Ashby, Brendon Hall, Chicheng Xu, Siddharth Misra, Weichang Li, Yan Xu, Oghenekaro Osogba


