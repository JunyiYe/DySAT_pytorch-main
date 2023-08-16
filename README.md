# DySAT: Deep Neural Representation Learning on Dynamic Graphs via Self-Attention Networks
This repository is cloned from https://github.com/FeiGSSS/DySAT_pytorch. I aim to use this implementation to test it on my own dataset.
This is a pytorch implementation of DySAT. All codes are adapted from official [implementation in TensorFlow](https://github.com/aravindsankar28/DySAT). This implementation is only tested using dataset Enron, and the results is inconsistent with official results (better than that). Code review and contribution is welcome!

# Raw Data Process
```
cd raw_data/Enron
pyhton process.py
```
The processed data will stored at 'data/Enron"

# Training
```
python train.py --dataset Enron --time_steps 16
```

# The result
```
Epoch 0  ,  Loss = 40.527, Val AUC 0.583 Test AUC 0.588
Epoch 1  ,  Loss = 28.977, Val AUC 0.639 Test AUC 0.616
Epoch 2  ,  Loss = 26.014, Val AUC 0.721 Test AUC 0.670
Epoch 3  ,  Loss = 24.267, Val AUC 0.774 Test AUC 0.719
Epoch 4  ,  Loss = 22.987, Val AUC 0.772 Test AUC 0.746
Epoch 5  ,  Loss = 21.793, Val AUC 0.776 Test AUC 0.776
Epoch 6  ,  Loss = 20.966, Val AUC 0.781 Test AUC 0.798
Epoch 7  ,  Loss = 20.216, Val AUC 0.794 Test AUC 0.816
Epoch 8  ,  Loss = 19.544, Val AUC 0.819 Test AUC 0.834
Epoch 9  ,  Loss = 19.052, Val AUC 0.845 Test AUC 0.844
Epoch 10 ,  Loss = 18.590, Val AUC 0.856 Test AUC 0.849
Epoch 11 ,  Loss = 18.243, Val AUC 0.872 Test AUC 0.855
Epoch 12 ,  Loss = 17.959, Val AUC 0.878 Test AUC 0.864
Epoch 13 ,  Loss = 17.681, Val AUC 0.883 Test AUC 0.871
Epoch 14 ,  Loss = 17.436, Val AUC 0.885 Test AUC 0.876
Epoch 15 ,  Loss = 17.267, Val AUC 0.886 Test AUC 0.880
Epoch 16 ,  Loss = 17.069, Val AUC 0.893 Test AUC 0.884
Epoch 17 ,  Loss = 16.900, Val AUC 0.900 Test AUC 0.888
Epoch 18 ,  Loss = 16.771, Val AUC 0.903 Test AUC 0.892
Epoch 19 ,  Loss = 16.705, Val AUC 0.906 Test AUC 0.895
Epoch 20 ,  Loss = 16.605, Val AUC 0.907 Test AUC 0.897
Epoch 21 ,  Loss = 16.550, Val AUC 0.911 Test AUC 0.899
Epoch 22 ,  Loss = 16.475, Val AUC 0.914 Test AUC 0.902
Epoch 23 ,  Loss = 16.376, Val AUC 0.917 Test AUC 0.905
Epoch 24 ,  Loss = 16.278, Val AUC 0.915 Test AUC 0.906
Epoch 25 ,  Loss = 16.242, Val AUC 0.914 Test AUC 0.908
Epoch 26 ,  Loss = 16.196, Val AUC 0.917 Test AUC 0.910
Epoch 27 ,  Loss = 16.138, Val AUC 0.914 Test AUC 0.911
Epoch 28 ,  Loss = 16.089, Val AUC 0.913 Test AUC 0.911
Epoch 29 ,  Loss = 16.042, Val AUC 0.913 Test AUC 0.911
Epoch 30 ,  Loss = 15.996, Val AUC 0.909 Test AUC 0.911
Epoch 31 ,  Loss = 15.939, Val AUC 0.903 Test AUC 0.911
Epoch 32 ,  Loss = 15.901, Val AUC 0.898 Test AUC 0.911
Epoch 33 ,  Loss = 15.848, Val AUC 0.897 Test AUC 0.910
Epoch 34 ,  Loss = 15.804, Val AUC 0.894 Test AUC 0.910
Epoch 35 ,  Loss = 15.783, Val AUC 0.893 Test AUC 0.911
Epoch 36 ,  Loss = 15.757, Val AUC 0.888 Test AUC 0.911
Best Test AUC = 0.910
```

