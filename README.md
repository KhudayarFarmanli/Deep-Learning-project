# MLDL-Final-Project
This project propose some extensions to improve Deep Visual Geo-Localization Benchmark ued for the task of VPR. The proposed extensions improve robustness to night images and occlusions, apply new optmizers for training the model, propose a multi-scale strategy for building richer descriptors and provide a way to combine models. Results are in `Results Analysis`

## Train Improvements
### Data Augmentation Night Robustness
- `datasets_augmented.py`: in this file we have define the data augmentation for night robustness with ColorJitter.
- `train_augmented.py`: we implement the train loop with this Color Jitter transformation.
- `datasets_constant.py`: in this file we have define the data augmentation for night robustness with Functional Adjust.
- `train_augmented_constant.py`:  we implement the train loop with this Functional Adjust transformation
### Data Augmentation Perspective
- `datasets_RP_RE.py`: in this file we have defined data augmentation for occlusions with Random Perspective and Random Erasing.
- `train_RP_RE.py`: we implement the train loop with these Random Perspective and Random Erasing transformations.
### Optimizers and Scheduler
- `train_optim.py`: in this file we have defined the training loop with the new optimizers: ADAMW and ASGD
- `train_optim_sched.py`: in this file we have defined the training loop with two schedulers: Cosine and Plateau.

## Test Improvements
### Multi-scale testing
- `test_impr.py`: in this file we have define the multi-scale pyramid  
### Ensemebling
- `test_ensam.py`: in this file we have defined the code for ensembling descriptors from different models
- `eval_impr.py`: in this file we implement both multi-scale and ensembling extensions for running it in the command line

## Vanilla model
- `commons.py`, `datasets_ws.py`, `eval.py`, `parser.py`, `test.py`, `train.py` and `util.py` and the folder `model` are the files from the original model.

## Project Description
[Data Augmentation.png](https://github.com/albertomg098/MLDL-Final-Project/issues/1#issue-1284023672)

[Multi-scale.png](https://github.com/albertomg098/MLDL-Final-Project/issues/1#issuecomment-1165804388)

[Ensembling.png](https://github.com/albertomg098/MLDL-Final-Project/issues/1#issuecomment-1165804191)
