## Vocabulary: 

#### Replication ratio: 
Ratio of L1 misses that can be found in other L1 caches to total L1 misses.
1. L1 Cache miss is basically: either the line is not present(tag-mismatch) or is invaid in my private L1.
2. Two cases exist here: 
* The requested line is not present in any other L1. (NO Replication)
* The requested line is present in atleast one other L1. (Replication exists)
4. In the total execution of a program, we want to count how many misses are of the later category.

Paper mentions: 
* C-BLK, C-RAY have low replication. 
* T-Alexnet, T-Resnet have very high replication.
