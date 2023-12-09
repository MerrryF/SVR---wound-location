# SVR---wound-location
CISC3023 Course Project

This is an SVR model for CISC3023 Course Project since the limited file size in UMoodle. Please download the SVR model from here for scoring.

Instruction of running SVR model:

    Platform of Running: Jupyter Notebook

    Preparation：
    a) Inicialize dataset information
       Reset the following variable as the path corresponding in the user's local disk:
       
       i. data_frame_train: Refers to the path of excel file "//Training//myData.csv" 
       ii. data_frame_test: Refers to the path of excel file "//Test//myData.csv" 
       iii. train_dir: Refers to the path of train image folder "//Training" 
       iv. test_dir: Refers to the path of test image folder "//Test" 
       v. aug_dir: Refers to the path of augmented image folder "//augmented"
    
    b) Training process
       The "SVR - trainer.ipynb" include all the features extraction method.
       After the users run all the codes sequentially, all the features visualization would be shown. 
       (Do not need to run "With convert" part when train the model, since it is not used as feature in the final model training.)
       
       After finish the section of "Train Model", user can obtain the training results with MSE loss and cross-validation results.
       The model will be save as "model.pkl" and the test data processed will also be saved for tester. 

    c) Testing process
       The "SVR - tester.ipynb" only include the test process without any feature extraction. 
       Tester will load the well saved model and test data files to perform the testing.
       User can obtain the testing results with MSE loss.

       If the user want to perform the results' visulization, you need to set the "test_images_folder" as the path of test image folder.
       Then all the visulization of performance will be shown in a folder named "performance-visualization" under the same path of "SVR - tester.ipynb".
