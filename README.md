# CS290-final-project
This is my final project for my computer vision class CS290

## HAM10000
The HAM10000 Dataset: A Large Collection of Multi-Source Dermatoscopic Images of Common Pigmented Skin Lesions
https://arxiv.org/abs/1803.10417

## Intro
This was a very fun and challenging project, especially because the dataset has been mainly trained with neural nets, rather than traditional methods that involve feature extraction. I used and tried different extraction approaches, and tried to classified with SVM and Random Forests. Overall, the biggest challenge was the very high class imbalance. However, I managed to deal with that through SMOTENN resampling. The notebook includes and exploratory data analysis, data preparation, feature extraction, training with traditional features. In the last part, I tried to add a new feature from the pre-trained ResNet18, which as can be seen will slightly improve the training accuracy. However, the best result will be achieved at the very end, with a Convolutional Neural Network.

Overall, this final project helped me to understand how to deal with a high class imbalance, how to extract features from images, how do apply dimensionality reduction, how to train using pre-trained model and finally how to implement a CNN using Pytorch.

## Skin Lesion Classification

### Project Overview
A deep learning model for classifying skin lesions into 7 different categories using a Convolutional Neural Network (CNN) built with PyTorch.

### Dataset
The model uses a dataset of skin lesion images with the following categories:

#### nv
Melanocytic nevi are benign neoplasms of melanocytes and appear in a myriad of variants, which all are included in our series. The variants may differ significantly from a dermatoscopic point of view.
[6705 images]

#### mel
Melanoma is a malignant neoplasm derived from melanocytes that may appear in different variants. If excised in an early stage it can be cured by simple surgical excision. Melanomas can be invasive or non-invasive (in situ). We included all variants of melanoma including melanoma in situ, but did exclude non-pigmented, subungual, ocular or mucosal melanoma.
[1113 images]

#### bkl
"Benign keratosis" is a generic class that includes seborrheic ker- atoses ("senile wart"), solar lentigo - which can be regarded a flat variant of seborrheic keratosis - and lichen-planus like keratoses (LPLK), which corresponds to a seborrheic keratosis or a solar lentigo with inflammation and regression [22]. The three subgroups may look different dermatoscop- ically, but we grouped them together because they are similar biologically and often reported under the same generic term histopathologically. From a dermatoscopic view, lichen planus-like keratoses are especially challeng- ing because they can show morphologic features mimicking melanoma [23] and are often biopsied or excised for diagnostic reasons.
[1099 images]

#### bcc
Basal cell carcinoma is a common variant of epithelial skin cancer that rarely metastasizes but grows destructively if untreated. It appears in different morphologic variants (flat, nodular, pigmented, cystic, etc) [21], which are all included in this set.
[514 images]

#### akiec
Actinic Keratoses (Solar Keratoses) and intraepithelial Carcinoma (Bowen's disease) are common non-invasive, variants of squamous cell car- cinoma that can be treated locally without surgery. Some authors regard them as precursors of squamous cell carcinomas and not as actual carci- nomas. There is, however, agreement that these lesions may progress to invasive squamous cell carcinoma - which is usually not pigmented. Both neoplasms commonly show surface scaling and commonly are devoid of pigment. Actinic keratoses are more common on the face and Bowen's disease is more common on other body sites. Because both types are in- duced by UV-light the surrounding skin is usually typified by severe sun damaged except in cases of Bowen's disease that are caused by human papilloma virus infection and not by UV. Pigmented variants exists for Bowen's disease [19] and for actinic keratoses [20]. Both are included in this set.
[327 images]

#### vasc
Vascular skin lesions in the dataset range from cherry angiomas to angiokeratomas [25] and pyogenic granulomas [26]. Hemorrhage is also included in this category.
[142 images]

#### df
Dermatofibroma is a benign skin lesion regarded as either a benign proliferation or an inflammatory reaction to minimal trauma. It is brown often showing a central zone of fibrosis dermatoscopically [24].
[115 images]

### Reference
Tschandl, Philipp. 2018. "The HAM10000 Dataset, a Large Collection of Multi-Source Dermatoscopic Images of Common Pigmented Skin Lesions." Harvard Dataverse. https://doi.org/doi:10.7910/DVN/DBW86T. 

### Contact
email: lucacharrouf@berkeley.edu


### Contact
email: [lucacharrouf@berkeley.edu](mailto:lucacharrouf@berkeley.edu)