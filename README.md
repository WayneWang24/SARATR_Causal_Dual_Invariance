# SARATR_Causal_Dual_Invariance
This is the official Pytorch implementation of Causal SAR ATR with Limited Data via Dual Invariance.

**Abstract:** SAR ATR with limited data has recently been a hot research topic to enhance weak generalization. 
Despite many excellent methods being proposed, a fundamental theory is lacked to explain what problem the limited SAR data causes, leading to weak generalization of ATR. 
In this paper, we establish a causal ATR model demonstrating that noise $N$ that could be blocked with ample SAR data, becomes a confounder with limited data. 
As a result, it has a detrimental causal effect damaging the efficacy of feature $X$ extracted from SAR images, leading to weak generalization of SAR ATR with limited data.
The effect of $N$ on feature can be estimated and eliminated by using backdoor adjustment to pursue the direct causality between $X$ and the predicted class $Y$.
However, it is difficult for SAR images to precisely estimate and eliminated the effect of $N$ on $X$. 
The presence of various interference types in SAR images, such as cluster and speckle, and the inter-class similarity of SAR images, which can be mistaken for the effect of $N$, complicates the precise estimation of $N$'s effect.
The limited SAR data hardly drives most existing ERM-based optimization losses, thus making it difficult to effectively eliminate $N$'s effect. 
To tackle with difficult estimation and elimination of $N$'s effect, we propose a dual invariance comprising the inner-class invariant proxy and the noise-invariance loss. 
Motivated by embracing change with invariance, the inner-class invariant proxy facilitates precise estimation of $N$'s effect on $X$ by obtaining accurate invariant features for each class with the limited data. 
The noise-invariance loss transitions the ERM's data quantity necessity into a need for noise environment annotations, effectively eliminating $N$'s effect on $X$ by cleverly applying the previous $N$'s estimation as the noise environment annotations.
Finally, the proposed causal ATR via dual invariance not only unravels the key problem caused by limited data, but also derives an effective principled solution.
Experiments on three benchmark datasets indicate that our proposed method achieves superior performance. 
Its effectiveness is further demonstrated through comprehensive ablation experiments.

The code and experiments are coming soon!
