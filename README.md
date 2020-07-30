# Active Learning Experiment Sampling 

This code does soft max experiment sampling for active learning applications. 

## Usage
All calls to the function are completed by inputting the correct predictive model followed by a sampling dataset, the overall goal of the active learning sampling, and optionally a β paramter, or the amine of choice and descriptor followed by the goal and a value for β. 
```bash
sample[model_ClassifierFunction, samplingDF_Dataset, goal_String, β_] 
sample[model_ClassifierFunction, amine_String, descriptor_String, goal_String, β_] 
```
Possible options for the goal include exploration and exploitation. Exploration chooses the next datapoint based solely on maximizing uncertainty, while exploitation favorably weights uncertain points with a higher True label probability. The beta parameter directly modulates the magnitude of this preferential sampling by increasing the entropy of points that are likely to be labelled as True. The beta parameter should be set to 0 if a goal other than exploit is chosen.
## Support
Any support related inquiries may be directed to wborrelli@fordham.edu. 

## Authors and Acknowledgement
Dr. Joshua Schrier, Kim B. and Stephen E. Bepler Chair of Chemistry at Fordham University, was immensely helpful in all aspects of this project. 
