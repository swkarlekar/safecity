# SafeCity Data
[SafeCity: Understanding Diverse Forms of Sexual Harassment Personal Stories](http://arxiv.org/abs/1809.04739), EMNLP 2018  
Authors: Sweta Karlekar & Mohit Bansal, University of North Carolina at Chapel Hill  

***This data is for research purposes only and is publicly available at <http://maps.safecity.in/reports>. Please contact SafeCity moderators at <http://maps.safecity.in/contact> for permission before the use of this data. We thank the SafeCity moderators for their assistance with the data download.***

See above for datasets with train, dev, and test splits used for binary and multi-label classification. 

## Single-Label Classification 

The data for single-label classification is given in two columns, with the first column being the description of the incident and the second column being 1 if the category of sexual harassment is present and 0 if it is not.   

*Examples from **Groping** Binary Classification Dataset:*   

| Description | Category |
|---|---|
| Was walking along crowded street, holding mums hand, when an elderly man groped butt, I turned to look at him and he looked away, and did it again after a while.I was 12 yrs old then. | 1 |
| This incident took place in the evening.I was in the metro when two guys started staring. | 0 |
| Catcalls and passing comments were two of the ghastly things the Delhi police at the International Airport put me and my friend through. It is appalling that the protectors and law enforcers at the airport can make someone so uncomfortable. |	0 |  
  
10% of each dataset was randomly selected and held-out for the test set. From the remaining training data, 10% was randomly selected and set aside for the development set. 

| Category | % Positive | 
|---|---|
| Commenting | 39.3% |
| Ogling | 21.4% |
| Groping | 30.1% |

For each category, there are 7201 training samples, 990 development samples, and 1701 test samples. 

## Multi-Label Classification 

The data for multi-label classification is given in four columns, with the first column being the description of the incident and the second, third, and fourth column being 1 if the category of sexual harassment is present and 0 if it is not.   

*Examples from **Multi-Label** Classification Dataset:*  

| Description | Commenting | Ogling/Facial Expressions/Staring | Touching/Groping |
|---|---|---|---|
| Was walking along crowded street, holding mums hand, when an elderly man groped butt, I turned to look at h7m and he looked away, and did it again after a while.I was 12 yrs old then. | 0 |	0 |	1 |
| This incident took place in the evening.I was in the metro when two guys started staring. |	0 |	1 |	0 |
| Catcalls and passing comments were two of the ghastly things the Delhi police at the International Airport put me and my friend through. It is appalling that the protectors and law enforcers at the airport can make someone so uncomfortable. | 1 |	1 |	0 |

10% of the dataset was randomly selected and held-out for the test set. From the remaining training data, 10% was randomly selected and set aside for the development set. 

| Commenting | Ogling | Groping | Examples in Dataset | 
|---|---|---|---|
| 1 | 1 | 1 | 351 | 
| 1 | 1 | 0 | 819 | 
| 1 | 0 | 1 | 459 | 
| 0 | 1 | 1 | 201 | 
| 1 | 0 | 0 | 2256 | 
| 0 | 0 | 1 | 1966 | 
| 0 | 1 | 0 | 743 | 
| 0 | 0 | 0 | 3097 | 

There are 7201 training samples, 990 development samples, and 1701 test samples.   

## Citation
If you find this dataset and code helpful, please consider citing [our paper](http://arxiv.org/abs/1809.04739).

```
@inproceedings{karlekar2018safecity,
	author = {Karlekar, Sweta and Bansal, Mohit},
	title = {SafeCity: Understanding Diverse Forms of Sexual Harassment Personal Stories},
	booktitle = {EMNLP},
	year = {2018},
}
```

## Questions?
Contact the authors of the paper at <swetakar@cs.unc.edu> and <mbansal@cs.unc.edu>. 
