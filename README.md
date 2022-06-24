# MLDL-Final-Project
This project propose some extensions to improve Deep Visual Geo-Localization Benchmark ued for the task of VPR. The proposed extensions improve robustness to night images and occlusions, apply new optmizers for training the model, propose a multi-scale strategy for building richer descriptors and provide a way to combine models.

## Analysis
Inside this folder (`Analysis`) there are some python files that has been used for a better understanding of the vanilla model. Inside it there are files that returns the size of an input dataset, some file thta analyze the dimensions of the descriptors, some file that analyze how packages inside torchvision.transforms works in an image, etc. This folder is not relevant for the final project but have decided to include it as a way of showing the previous analysis we have made before coding the final version of the project.
## Test Improvements
- The implementation of the multi-scale testing extension is defined in `test_multiscale.py`
- The implementation of the ensembling extension is defined in `test_ensemble.py`
- Finally, in eval it is specified whether to use test_multiscale or test_ensemble thanks to flags defined in `parser.py`

## Project Description
[Data Augmentation 2.png](https://github.com/albertomg098/MLDL-Final-Project/issues/1#issue-1284023672)](https://github.com/albertomg098/MLDL-Final-Project/issues/1#issue-1284023672)

[Multi-scale.png](https://github.com/albertomg098/MLDL-Final-Project/issues/1#issuecomment-1165804388)

[Ensembling.png](https://github.com/albertomg098/MLDL-Final-Project/issues/1#issuecomment-1165804191)
