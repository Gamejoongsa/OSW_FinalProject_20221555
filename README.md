# OSW_FinalProject_20221555
## OpenSourceSW Course Final Project - Brain Tumor MRI Classification
* This program shows the process of learning AI that receives and classifies Brain Tumor MRI images.
### Configuration instructions
#### Training Dataset
* Brain Tumors are classified as: Benign Tumor, Malignant Tumor, Pituitary Tumor, etc.
* There are four classes for training dataset : _glimora_tumor, meningioma_tumor, pituitary_tumor, and no_tumor._
* All datas are in the <U>tumor_dataset<U> folder.
* Each folder has more four subfolders.
  * These folders have MRIs of respective tumor classes.
  
#### Used Algorithms
* Random Forest
* Multi-Layer Perceptron
* K-Neighbors
* Support Vertor Machine
* Stacking Ensemble
  
#### Hyperparameters of the function
* Random Forest
'''Python
   rf_clf = sklearn.ensemble.RandomForestClassifier(criterion='gini',
                                             n_estimators=4096,
                                             random_state=0)
 '''
* Multi-Layer Perceptron
'''Python
  mlp_clf = MLPClassifier(max_iter=1500,
                    hidden_layer_sizes=(30, 20, 15),
                    activation='relu',
                    learning_rate='adaptive',
                    alpha=0.001,
                   random_state=0)
'''
* Multi-Layer Perceptron
 '''Python 
  svc_clf = sklearn.svm.SVC(C=10.0,
                      gamma=0.01,
                      random_state = 0)
'''
* Multi-Layer Perceptron
 '''Python 
  knn_clf = KNeighborsClassifier(n_neighbors=4,
                           algorithm='auto',
                           weights='distance')
  '''
* Multi-Layer Perceptron
 '''Python 
  meta_clf = sklearn.linear_model.LogisticRegression(max_iter=1500,
                                              random_state=0)
  '''
  
### Operating instructions
> Just open the .ipynb file and run
### Copyright and licensing information
> All copyrights and licenses are subject to MIT License.
### Contact information for the distributor or author
> E-mail : jane10000@cau.ac.kr
