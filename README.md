# Deep Learning In Medicine 
## Classifying Melanoma on Cloudera Machine Learning   


### Summary

1. Take open source images of skin lesions, and use those to build a classifier to detect malignant skin lesions
2. Evaluate the performance of the model using TensorBoard, and matplotlib in CML
3. Deploy the model onto a mobile device for use in clinical settings
4. Use the mobile app to determine if a patient needs critical attention from a physician (Note: in the demo we use a model deployed on a mobile device, for simplicity.  I.e. inference happens on the edge, using a low latency, MobileNet model.  The more likely choice for this use case would be to perform classification in batch or perform the inference centrally, using a model with superior performance characteristics (measured by AUC).

### 1.

![](images/ISIC.PNG)

### 2.
![](images/TensorboardGraphs.PNG)


### 3.
![](images/TensorboardHistograms.PNG)


### 4.

![](images/Mobile.PNG)


## Talk Tracks (Preliminary):

- [Deck and Demo Talk Track](https://rebrand.ly/6t1d66b)


## Deck:

- [De](https://rebrand.ly/nrdz1m)[ck](https://rebrand.ly/nrdz1m)



## Demo Setup

The setup takes 5 minutes



#### 1. 

In CML Go to Projects, and create a New Project

 

![](images/CreateProject.PNG)

 


#### 2. 

Name the Project "Melanoma Classification", and in the initial setup use git repo: 
https://github.com/hortonworks-sk/CML-Classifying-Melanoma.git, 
and hit the create button



![](images/CreateProject2.PNG)



#### 3. 

Launch a Python 3 workbench session


![](images/OpenWorkBench.PNG)


#### 4. 

Navigate to the load-libraries.sh script, and run the script. This will load the libraries needed for the demo.


![](images/OpenWorkBench2.PNG)



#### 5. 

Navigate to the start_tensorboard.py script, and run this.  


![](images/StartTensorboard.PNG)


#### 6.

Check that the Tensorboard link is displaying in CDSW and that tensorboard is running, by clicking the tensorboard link



![](images/OpenTensorboard.PNG)


#### 7. 

Click on the tensorboard tabs for Scalars , Graph and the Histograms , to check that these are displaying correctly (each are shown in order below)


![](images/TensorboardGraphs.PNG)


![](images/TensorboardScalars.PNG)


![](images/TensorboardHistograms.PNG)


#### 8. 

Navigate to experiments and click run experiment


![](images/Experiments.PNG)


#### 9. 

Run experiments for the **_Inception3.py , and ** _VGG16.py**, scripts.  Use the python 3 kernel. No need to supply arguments for these. 

![](images/Experiments-Inception.PNG)



#### 10. 

When these runs have completed, you should see the experiments listed as successful in the experiments view (as in the screenshot below)



![](images/Experiments-List.PNG)



### Pre-Demo Setup

Having the following tabs open, in a Chrome window, may be useful (these are the tabs open in the talk track video):


1.  The ISIC dataset homepage (https://www.isic-archive.com/#!/topWithHeader/wideContentTop/main)


2.  The CDSW file view of the training data folder http://your-cdsw-host.and-domain.com/yourusername/melanoma-classification/files/demo/data/test/   (This is at the folder path:    demo > data > test  in CDSW)


![](images/DataFolders.PNG)



3.  A Python 3 workbench session (loaded within the Classifying Melanoma project) pointing to the script to train the classifier  (This is at the path:    demo > models > classifier3.py, in CDSW)


![](images/CDSWSession_Classifier.PNG)


4.  Tensorboard, with the Graph view 



![](images/TensorboardGraphs.PNG)



5.  The new Projects http://your-cdsw-host.and-domain.com/projects/new


![](images/CDSWSession_Classifier.PNG)



6.  The experiments page


7.   http://[your-cdsw-host.and-domain.com]/projects/new/[your-username]/mel2/runs admin/mel2/runs



### Use Case & Industry Applicability

- Use Case:  Diagnosing Melanoma
- Broader Healthcare Applicability:
  - Disease diagnosis using medical images
    - radiology (arteriography, mammography, radiomics)
    - dermatology
    - oncology

- Broader Industry applicability
  - Biotech
  - Pharma
  - Semiconductor Fabrication

