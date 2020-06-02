
The purpose of this ODIR challenge is to compare approaches of ophthalmic disease classification in color fundus images. Dataset comprises of images of 5000 patients categried into into eight labels including normal (N), diabetes (D), glaucoma (G), cataract (C), AMD (A), hypertension (H), myopia (M) and other diseases/abnormalities (O)
![image distribution](https://grand-challenge-public.s3.amazonaws.com/i/2020/01/21/be3b0252.png)


# Final Notebooks
[working_2.ipynb](https://github.com/talhaanwarch/ODIR2019/blob/master/working_2.ipynb) is the final solution that i submitted. In this notebook we used two paralel EfficientNetB3 architecture one for each eye side. Focal loss is used as loss function and adam as optimizers. 

# Scores
"kappa": 0.5198645332075835,
"AUC_vlaue": 0.9078637702944817,
"f-1_score": 0.8599999999999999,
"Final_Score": 0.7625761011673551


Following are the sources that help me alot while doing this 
https://www.kaggle.com/c/human-protein-atlas-image-classification/discussion/75691  
https://www.kaggle.com/c/human-protein-atlas-image-classification/discussion/70365  
https://www.kaggle.com/c/human-protein-atlas-image-classification/discussion/74374
https://shaoanlu.wordpress.com/2018/03/26/experiment-with-group-normalization/
