# Bird-Song-Recognition-SVM-Scikit-Learn

The presence of birds in a habitat has long since been used as a measure of biodiversity. Previously a trained person would sit
in the habitat and manually record the bird they heard by the song.
Subsequently recording devices were left in the habitats of concern and trained personnel would listen to the recordings from
an office and manually record which birds were heard.
Both of these approaches require having having trained personnel who are able to distinguish between different bird calls
accurately and is also very labour intensive.
Machine learning has the potential to:
• Increase the accuracy of the classification of bird species.
• Decrease the time needed to classify what birds are present in a habitat.
• Decrease the expense of bird song classification.
• Be an non-invasive way of detecting species including nocturnal species.

## Data and Model Structure
A dataset of acoustic features which had been extracted from each audio clip.
136 features of each clip were extracted as used for the inputs in this approach.

An SVM was trained on these features to recognise the species. 
One main advantage of this model is the trade off between computational cost and accuracy is pretty good. The model was able
to achieve 69.29% accuracy with less than 7 seconds training time.
This could particularly be an advantage if the model was going to be trained on a much larger training set and computational
resources were limited.

### Varying by Location/Season
One possible improvement which we inspected was to vary the model depending on the location/habitat.
Each model was then trained only using birds typically found in each habitat. The best results were again obtained from the
SVM. It is possible to achieve greater accuracy for these models
