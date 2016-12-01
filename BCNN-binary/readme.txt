===============================================================================
Model_1:
BCNN with binary values (+1 and -1, padded value is +1):
File:		CifarBCNN_1.npz
Structure:	
Full Conv layer: (128-128-256-256-512-512)
Full FC layer: (1024-1024-10)
Preserve all bias; (for both FC and CONV layers)

Performance on cifar-10 Testing dataset:
Error rate:
11.70% (1170 of 10000)
original BCNN: about 11.40%

parameter size: same as original BCNN, about 13.6M bits


===============================================================================
Model_2:
BCNN with binary values (+1 and -1, padded value is +1), and delete all bias:
File:		CifarBCNN_2.npz
Structure:	
Full Conv layer: (128-128-256-256-512-512)
Full FC layer: (1024-1024-10)
Delete all bias; (for both FC and CONV layers)

Performance on cifar-10 Testing dataset:
Error rate:
11.81% (1181 of 10000)
parameter size: almost same as original BCNN, about 13.6M bits


===============================================================================
Model_3:
BCNN with binary values (+1 and -1, padded value is +1), and delete all bias:
File:		CifarBCNN_3.npz
Structure:	
Full Conv layer: (128-128-256-256-512-512)
Reduce FC layer: (128-10)
Delete all bias; (for both FC and CONV layers)

Performance on cifar-10 Testing dataset:
Error rate:
12.20% (1220 of 10000)

parameter size: about 5.9M bits
