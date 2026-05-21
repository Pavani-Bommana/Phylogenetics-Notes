
<img width="681" height="342" alt="image" src="https://github.com/user-attachments/assets/0d4b99c2-0448-4b93-9bbb-4a2546a44850" />

# Method Classification Schema

## 1. Non-Parametric Methods
These methods do not use an explicit probabilistic model of sequence evolution to evaluate trees. Most of these methods calculate a distance and continue in a pairwise manner through the whole set of sequences. 
<img width="2116" height="105" alt="image" src="https://github.com/user-attachments/assets/a3098d36-3857-4da9-a94d-3cca0814264c" />


* **Distance-Based (Clustering Algorithms):**
    * **UPGMA:** Fast clustering that assumes a strict molecular clock (produces ultrametric trees).
    * **Neighbor-Joining (NJ):** Fast clustering that allows for unequal rates of evolution among lineages.
* **Parsimony-Based (Optimization Criteria):**
    * **Maximum Parsimony (MP):** Evaluates character states directly to find the tree requiring the fewest total mutations.

---

## 2. Parametric Methods
These methods are entirely model-based, utilizing complex statistical parameters to calculate tree probabilities site-by-site that means take a column in an alignment and calculate the optimality criterion per position in alignment and assumes positions are independent. 
<img width="2128" height="105" alt="image" src="https://github.com/user-attachments/assets/d212f4b3-67e6-450e-a60c-dd22c4f5f555" />
 .

* **Maximum Likelihood (ML):** Evaluates the data to find the single tree topology that maximizes the likelihood function ($L = P(\text{Data} \mid \text{Tree, Model})$).
* **Bayesian Inference (BI):** Uses MCMC to estimate the posterior probability distribution of trees ($P(\text{Tree} \mid \text{Data, Model})$).
