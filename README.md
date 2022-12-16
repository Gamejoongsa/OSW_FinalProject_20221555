# OSW_FinalProject_20221555
## OpenSourceSW Course Final Project - Brain Tumor MRI Classification
* This program shows the process of learning AI that receives and classifies Brain Tumor MRI images.
### Configuration instructions
#### Training Dataset
* Brain Tumors are classified as: Benign Tumor, Malignant Tumor, Pituitary Tumor, etc.
* There are four classes for training dataset : _glimora_tumor, meningioma_tumor, pituitary_tumor, and no_tumor._
* All datas are in the `tumor_dataset` folder.
* Each folder has more four subfolders.
  * These folders have MRIs of respective tumor classes.
* **Splited Training and Test datasets ratio is set to 0.3 -> 0.01. <--Important!** 
  
#### Used Algorithms
* Support Vertor Machine
  
#### Hyperparameters of the function
* Code of Support Vertor Machine 
```Python
clf = sklearn.svm.SVC(C=56.66691242696504,
                       gamma=1.1816539689843626,
                       probability=True,
                       random_state=3868671)
```
* Explaining of Parameters
  - `C` : Regularization parameter. The strength of the regularization is inversely proportional to C. Must be strictly positive. The penalty is a squared l2 penalty.
  - `gamma` : Kernel coefficient.
  - `probability` : Whether to enable probability estimates. This must be enabled prior to calling `fit`, will slow down that method as it internally uses 5-fold cross-validation, and `predict_proba` may be inconsistent with `predict`.
  - `random_state` : Controls the pseudo random number generation for shuffling the data for probability estimates.

### Operating instructions
* Fork this repository, or download `tumor_dataset` folder and `.ipynb` file.
* Then just open the `.ipynb` file and run
### Copyright and licensing information
* All copyrights and licenses are subject to `MIT License`.
[See more details](https://github.com/Gamejoongsa/OSW_FinalProject_20221555/blob/master/LICENSE)
### Contact me
> Name : Jaein Lee

> Student ID : 20221555

> E-mail : jane10000@cau.ac.kr
