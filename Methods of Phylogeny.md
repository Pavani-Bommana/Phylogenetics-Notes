
<img width="681" height="342" alt="image" src="https://github.com/user-attachments/assets/0d4b99c2-0448-4b93-9bbb-4a2546a44850" />

# Method Classification Schema

## 1. Non-Parametric Methods
These methods do not use an explicit probabilistic model of sequence evolution to evaluate trees. Most of these methods calculate a distance and continue in a pairwise manner through the whole set of sequences. 


* **Distance-Based (Clustering Algorithms):**
    * **UPGMA:** Fast clustering that assumes a strict molecular clock (produces ultrametric trees). It pairs the most similar sequences first, averages their distance to the next closest sequence, and builds the tree from the tips back to the root. It forces the tree to be ultrametric, meaning it assumes a strict              "molecular clock" where all lineages evolve at the exact same speed.
    * **Neighbor-Joining (NJ):** Fast clustering that allows for unequal rates of evolution among lineages. this does not assume molecular clock.
* **Parsimony-Based (Optimization Criteria):**
    * **Maximum Parsimony (MP):** Evaluates character states directly to find the tree requiring the fewest total mutations. A site-by-site analysis method that focuses on minimizing the total evolutionary path.

---

## 2. Parametric Methods
These methods are entirely model-based, utilizing complex statistical parameters to calculate tree probabilities site-by-site that means take a column in an alignment and calculate the optimality criterion per position in alignment and assumes positions are independent. 

* **Maximum Likelihood (ML):** Evaluates the data to find the single tree topology that maximizes the likelihood function.
* **Bayesian Inference (BI):** Uses MCMC to estimate the posterior probability distribution of trees.
* Both methods:
Search tree space to find the best tree
Require an explicit model of evolution
Can incorporate rate heterogeneity


