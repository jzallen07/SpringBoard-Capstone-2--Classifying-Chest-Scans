
# Springboard-Capstone-2-X-Ray Classification
using machine learning to screen x-rays for pathology

## Background

<ceneter><img src="/images/3_scan" alt="example images"></center>

Many thousands of x-rays are performed daily. Within the medical community the assessment of an x-ray especially a chest x-ray (CXR), at least in the rapid screening since is a highly common if not ubiquitous task amounts many medical specialties. Official review is done by a Radiologist (MD or DO). To them this task routine in most cases due to the fact that they have evaluated so many. However, to get to that point they have had to undergo many years of school and residency. In addition to this, despite being a minor task, the sheer number of them requries significant amounts of time which can be taxing on the system. 


## Data

From the NIH X-ray dataset found <a href="https://www.nih.gov/news-events/news-releases/nih-clinical-center-provides-one-largest-publicly-available-chest-x-ray-datasets-scientific-community">here</a>. This dataset contains some 112,120 thoracic scans from 30 or so tousand patients. They have labeled using NLP techniques based on findings in the relevant health records. It should be noted that the accuracy of these labels has been brought into question by many individuals.  

## Methodology

Use a transitional model neural network (deep learning model) to classify images based upon the provided label. Specifically the ResNet50 base with several custom layers on top will be used. Keras was used with a TensorFlow backend. 

## Conclusion

<ceneter><img src="/images/roc_1.png" alt="performance"></center>

The resulting model performed with similar performance to those described <a href="http://openaccess.thecvf.com/content_cvpr_2017/papers/Wang_ChestX-ray8_Hospital-Scale_Chest_CVPR_2017_paper.pdf">here</a>. Although, it should be noted that 9 categories were used there and 15 were used in this exercise. 

<ceneter><img src="/images/img_predictions.png" alt="prediction results"></center>
