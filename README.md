# Ocular Disease Intelligent Recognition (ODIR-2019)
The purpose of this ODIR challenge is to compare approaches of ophthalmic disease classification in color fundus images. Dataset comprises of images of 5000 patients categried into into eight labels including normal (N), diabetes (D), glaucoma (G), cataract (C), AMD (A), hypertension (H), myopia (M) and other diseases/abnormalities (O)
![image distribution](https://grand-challenge-public.s3.amazonaws.com/i/2020/01/21/be3b0252.png)


# Final Notebooks
[working_2.ipynb](https://github.com/talhaanwarch/ODIR2019/blob/master/working_2.ipynb) is the final solution that i submitted. In this notebook we used two paralel EfficientNetB3 architecture one for each eye side. Focal loss is used as loss function and adam as optimizers.   
[tpu-odir.ipynb](https://github.com/talhaanwarch/ODIR2019/blob/master/tpu-odir.ipynb) is the TPU verison which made us capable of training or large image size and batch size. Unlike the [working_2.ipynb](https://github.com/talhaanwarch/ODIR2019/blob/master/working_2.ipynb) implementation which used tensorflow < 2 , TPU version is trained with tensorflow>= 2.0. Kaggle TPU is used for this task. To rerun the notebook, fork it on kaggle  [here](https://www.kaggle.com/chtalhaanwar/tpu-odir) .

# Scores

"kappa": 0.5484336363210259,  
"AUC_vlaue": 0.9167666361765955,   
"f-1_score": 0.90125,  
"Final_Score": 0.7888167574992071  

# Acknowledgement 
Following are the sources that help me alot while doing this   
https://www.kaggle.com/c/human-protein-atlas-image-classification/discussion/75691  
https://www.kaggle.com/c/human-protein-atlas-image-classification/discussion/70365  
https://www.kaggle.com/c/human-protein-atlas-image-classification/discussion/74374
https://shaoanlu.wordpress.com/2018/03/26/experiment-with-group-normalization/
