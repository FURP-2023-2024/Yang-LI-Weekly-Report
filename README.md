# Yang-LI-Weekly-Report
## Week 1
Read relative papers about the tactip and reviewed the previous data analysis methods.
## Week 2 
Processing the data and extracting features from a sample video to determine the displacement using the optical flow method
## Week 3
Read another 3 papers about gelsight and built some general deep learning neural networks.
## Week 4 to week 10
run basic CycleGan, STSGCN, ECC. 
Using 2 high-speed cameras to capture the small changes between each frame, called vibrations in physics. After that, I used LK Optical Flow and contour recognition to determine those vibrations and recorded the average displacement of each contour in each frame. Then, I labelled each frame with a certain scale and got a dataset (label: scale, feature: average displacement of each contour in each frame). Finally, machine learning and deep learning models were used to train this dataset and predict the labels successfully in a testing video. After trying most of the models, I found when the KNN and GradientBoostingRegressor models were applied together, the predicted results were close to the real ones and the mean squared error was below 0.45.
improve the whole algorithm to ensure that the label corresponding to each frame is predicted within 2ms.
