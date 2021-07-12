TOPSIS
===================

Perform TOPSIS on different models to rank them depending on the weights and impact of each parameters.



Documentation
-------------

Commands:

1.   import topsis_vinay_101803108 as top
2.   top.topsis("filename","wts list","impacts list","resultfile")

> **Note:**

>-  File should be of CSV type containing all the parameter for different files.
>- Provdie weights and impact array in form of list
>- wts => [1,1,1,1], impacts => ['-','+','+','+']

Eg.

After Analysing 

top.topsis('file.csv',[1,1,0,5,1],['+','+','-','+'],'out.csv')

| Model | Corr | Rseq | Rmse | Accuracy | T_score | Rank |
|-------|------|------|------|----------|---------|------|
| M1    | 0.79 | 0.62 | 1.25 | 60.89    | 0.32358 |   2  |
| M2    | 0.66 | 0.44 | 2.89 | 63.07    | 0.29871 |   3  |
| M3    | 0.56 | 0.31 | 1.57 | 62.87    | 0.59283 |   1  |


