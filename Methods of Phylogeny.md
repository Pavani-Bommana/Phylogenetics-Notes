
<img width="681" height="342" alt="image" src="https://github.com/user-attachments/assets/0d4b99c2-0448-4b93-9bbb-4a2546a44850" />

# Method Classification Schema

## 1. Non-Parametric Methods
These methods do not use an explicit probabilistic model of sequence evolution to evaluate trees.

* **Distance-Based (Clustering Algorithms):**
    * **UPGMA:** Fast clustering that assumes a strict molecular clock (produces ultrametric trees).
    * **Neighbor-Joining (NJ):** Fast clustering that allows for unequal rates of evolution among lineages.
* **Parsimony-Based (Optimization Criteria):**
    * **Maximum Parsimony (MP):** Evaluates character states directly to find the tree requiring the fewest total mutations.

---

## 2. Parametric Methods
These methods are entirely model-based, utilizing complex statistical parameters to calculate tree probabilities site-by-site.

* **Maximum Likelihood (ML):** Evaluates the data to find the single tree topology that maximizes the likelihood function ($L = P(\text{Data} \mid \text{Tree, Model})$).
* **Bayesian Inference (BI):** Uses MCMC to estimate the posterior probability distribution of trees ($P(\text{Tree} \mid \text{Data, Model})$).
