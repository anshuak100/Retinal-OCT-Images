# Retinal-OCT-Images
to detect and classify human diseases from medical images.

<h2> Description </h2>

The dataset is organized into 3 folders (train, test, val) and contains subfolders for each image category (NORMAL,CNV,DME,DRUSEN). There are 84,495 X-Ray images (JPEG) and 4 categories (NORMAL,CNV,DME,DRUSEN).

Images are labeled as (disease)-(randomized patient ID)-(image number by this patient) and split into 4 directories: CNV, DME, DRUSEN, and NORMAL.

Optical coherence tomography (OCT) images (Spectralis OCT, Heidelberg Engineering, Germany) were selected from retrospective cohorts of adult patients from the Shiley Eye Institute of the University of California San Diego, the California Retinal Research Foundation, Medical Center Ophthalmology Associates, the Shanghai First People’s Hospital, and Beijing Tongren Eye Center between July 1, 2013 and March 1, 2017.

<h2> Source / useful links </h2>

DataSource : https://www.kaggle.com/paultimothymooney/kermany2018 <br>
Citation : http://www.cell.com/cell/fulltext/S0092-8674(18)30154-5

<h3> Type of Machine Learning Problem</h3>

<p> It is a one class classification problem, for a given image we need to predict if they are suffering from which disease. </p>

<h3> Performance Metric </h3>

Metric(s): 
* Categorical Crossentropy
* Confusion Matrix

<h3> How does it work ? </h3>
* Understanding image data
* Image augmentation
* Applying model

<h3> Conclusion </h3>
1. we applied image augmentation to this dataset.<br>
2. we applied three model - InceptionNet, DenseNet, and ResNet. <br>
3. we have taken the weight of every model which is trained on imagenet dataset, we have not freezed the layer because the retina dataset is different from imagenet dataset.<br>
4. we used confusion matrix because dataset is imbalanced and so accuracy score may not give good sence of result.<br>
5. By seeing the confusion matrix of all the three model we can say that inception net has best recall  than other model, precision is also good for inception net.
