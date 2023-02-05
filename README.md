# Face Recognition
Face Recognition using PCA and Robust PCA. 


The main goal of this repository is to visualize and understand an application of the Principal Component Analysis (PCA) algorithm and how it works in the background. Then RPCA is used to find the sparse errors areas of objective faces and the math behind it is discussed.  
The algorithms is tested on synthetic data as well as the original research paper dataset ( [YaleB dataset](https://www.kaggle.com/datasets/olgabelitskaya/yale-face-database) ). At last both PCA  and RPCA are tested on lfw-people dataset for different cases including original case and noisy case by adding gaussian, salt&pepper and speckle noise.


Dataset : [LFW - People (Face Recognition)](https://www.kaggle.com/datasets/atulanandjha/lfwpeople)

Test on dataset : `RPCA_FaceRecognition.ipynb`. 

Robust PCA : `robust_pca.py`




## Robust PCA
Face recognition is a problem domain in computer vision where low-dimensional linear models have received a great deal of attention. However, since faces are not perfectly convex, real face images often violate low-rank model, due to cast shadows and specularities. These errors are large in magnitude, but sparse in the spatial domain. It is reasonable to believe that if we have enough images of the same face, RPCA  will be able to remove these errors.  


The goal of Robust PCA is D = A + E . This goal can be best illustrated with the image below:  

![image](https://kojinoshiba.com/assets/images/2018-05-27-robust-pca/robust_pca.png) 


Face Recognition using RPCA Demo test on LFW - People dataset:  

[![image](https://www.linkpicture.com/q/download3_1.png)](https://www.linkpicture.com/view.php?img=LPic63dd698bbe49b1061729209)





## Reference 

- [RPCA Research Paper](https://arxiv.org/pdf/0912.3599.pdf) : Candès et al. in 2011
- [RPCA Implementation](https://github.com/dganguli/robust-pca)
- [Mathematical interpretation](https://kojinoshiba.com/pca/)











