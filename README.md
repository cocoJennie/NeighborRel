# NeighborRel
Original Gaitset work with RelPascksequence achieves surprise results. 
This repo is used for interpret the surprising performance.


## exp summaries
2023/11/17:
1. dataset shuffle: PS(PackSequence) won't change; RelPS changed on the **sample-wise shuffle**, keep consistency on the group wise shuffle. [Reasonable]





## fixed bug hauls
2023/11/17:
1. shuffle should be down in dataset instead of sampler in the inference stage. SINCE the label information is directly form the dataset, it is disentangled with the sampler indices shuffling. 