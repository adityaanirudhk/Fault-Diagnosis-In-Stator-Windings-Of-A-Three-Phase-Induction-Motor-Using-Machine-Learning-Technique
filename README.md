# Early-Stage-Fault-Detection-of-Stator-Winding-in-3-phase-Induction-Motor-using-Machine-Learning
First of all we have collected data and exported in data sheet.we have collected the data for healthy, unbalance, Faulty(stator winding) motor by doing an experiment and all of the data has been collected by YOKOGOWA power analyser. The collected data is stator current of three phases.For making the anaysis simplier we have converted the all 3 phase data into a single one by doing park's vector method. For ML Algorithms we need to select some of the feature  We have done Feature extraction(33 feature) from PVM and PVAC . We have trained and tasted the model choosen classifier by giving 75% data for traning and we have used 25% data for testing out of180 sample. Then choose the best classifier and the best classifier that we get is K-Nearest Neighbour. After selecting the best model we have to tune the parameter of KNN model so that we get best accuracy. After fitting test data into the model we get accuracy of 91.1% and we can see the confusion matrix that shows how well the model classified the different fault (Healthy(0), Unbalance(1), Stator fault(2)) of motor . Out of 15 healthy test data all 15 are predicted in heathy class, out of 15 unbalance data 13 samples are classified in unbalance class and other 2 are misclassified in faulty case, out of 15 stator fault data 13 samples are classified in fault class and other 2 are misclassified in unbalance case.