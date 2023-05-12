# Problem Statement
Authentication is a crucial factor for managing security. Signatures are widely used for personal identification and verification in various documents, such as legal transactions and bank cheques. Signature-based verification of multiple documents is a time-consuming and difficult task. Consequently, biometric personal verification and authentication systems have gained popularity as traditional identity verification methods like passwords, tokens, and pins suffer from some fatal flaws and are incapable of satisfying security necessities.

This project aims to identify whether a handwritten signature is real or forged and detecting the signature in a document. The project is divided into two parts, and the datasets for each part are described below.

# Part 1 - Signature Verification Dataset
The Signature Verification Dataset can be found [here](https://drive.google.com/file/d/1WqIhqp9JJ65SZPs9v868P_-SBCVTR2By/view). The dataset consists of 5 subfolders, and each subfolder contains train and test folders for a particular person (Person A to Person E).

Each train folder contains 40 images, and each test folder contains 8 images of a particular person's signatures. Along with the images, each train and test folder has a CSV file containing signature verification labels.

The task is to create a single Siamese model and report the test accuracy on the 40 test images.

# Part 2 - Object Detection Dataset
The Object Detection Dataset can be found [here](https://drive.google.com/file/d/1gew1zSfSZKiUKGPGc3bpGXbO03HvE9-_/view). The dataset consists of four folders:

- TrainImages: Contains 660 training images for the detection task.
- TrainGroundTruth: Contains 660 corresponding detection labels for the training detection task. Each image in the TrainImages folder has a corresponding text file in this folder with the same name as the image. The text file has (1 or more) rows, where each row represents the bounding box of a single signature. Each row has 4 values: x1, y1, x2, y2.
- TestImages: Contains 115 testing images for the detection task.
- TestGroundTruth: Contains 115 corresponding detection labels for testing the detection task.
 
The objective of this part is to detect signatures in the given images using the training set and report the results on the testing set.

# Conclusion
This project aims to help develop signature detection and verification methods to improve security measures. The datasets provided in this project can be used to create and train models for signature verification and object detection tasks.
