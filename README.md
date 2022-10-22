# aaai2023
aaai2023 rebuttal
# Weakness 1，3,and 5:
You are very knowledgeable. LEAP[2] and OFA[3] are among the pioneers of head-to-tail knowledge transfer, which we have discussed in related work. We have shown the performance of FUR with decoupled training in Table 4 and OFA with decoupled training in Table 3, and we can observe that the overall performance of our approach is 19.6% and 6.2% higher than OFA on ImageNet-LT and iNaturalist2018, respectively. Based on your suggestion, we supplemented the performance when FUR, OFA, and LEAP are all trained with three stages, and the results are as follows.

|      | ImageNet-LT | iNaturalist2018 |
|------|-------------|-----------------|
| LEAP | 43.7%       | 65.8%           |
| OFA  | 36.4%       | 67.2%           |
|  FUR | 55.1%       | 72.3%           |

[2] Deep Representation Learning on Long-tailed Data: A Learnable Embedding Augmentation Perspective [3] Feature Space Augmentation for Long-Tailed Data

# Weakness2: 
Following the accepted settings, the batch size on ImageNet-LT and iNaturalist2018 is 256 and 512, respectively. For a fair comparison, we align with OFA and choose N_A to be 3, so N_T is 32 and 64 on ImageNet-LT and
iNaturalist2018, respectively.

# Weakness 4: 
We argue that although the bias of the classifier is improved after decoupled training, the ability of the feature sub-network to adapt to the new decision boundary is ignored.
