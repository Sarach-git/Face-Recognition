# Face Recognition
Face Recognition using PCA and Robust PCA. 


The main goal of this repository is to visualize and understand an application of the Principal Component Analysis (PCA) algorithm and how it works in the background. Then RPCA is used to find the sparse errors areas of objective faces and the math behind it is discussed. 


Dataset : [LFW - People (Face Recognition)](https://www.kaggle.com/datasets/atulanandjha/lfwpeople)

Test on dataset : `RPCA_FaceDeection.ipynb` 

RPSA :`RPCA.py` 


## Robust PCA
Face recognition is a problem domain in computer vision where low-dimensional linear models have received a great deal of attention. However, since faces are not perfectly convex, real face images often violate low-rank model, due to cast shadows and specularities. These errors are large in magnitude, but sparse in the spatial domain. It is reasonable to believe that if we have enough images of the same face, RPCA  will be able to remove these errors.  


The goal of Robust PCA is D = A + E . This goal can be best illustrated with the image below:  

![image](https://kojinoshiba.com/assets/images/2018-05-27-robust-pca/robust_pca.png). 




## Reference 

- [RPCA Research Paper](https://arxiv.org/pdf/0912.3599.pdf) : Candès et al. in 2011
- [RPCA Implementation](https://github.com/dganguli/robust-pca)
- [Mathematical interpretation](https://kojinoshiba.com/pca/)











