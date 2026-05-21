Phylogenetic Methods
  graph TD
    PM[Phylogenetic Methods] --> NP[NON-PARAMETRIC<br>No statistical model/parameters]
    PM --> P[PARAMETRIC<br>Explicit model/parameters]
    
    NP --> DB[Distance-Based<br>Matrix inputs]
    NP --> PB[Parsimony-Based<br>Character inputs]
    
    DB --> UPGMA[UPGMA]
    DB --> NJ[Neighbor-Joining NJ]
    PB --> MP[Maximum Parsimony MP]
    
    P --> ML[Maximum Likelihood ML]
    P --> BI[Bayesian Inference BI]
    
    ML --> ML_Soft[e.g., IQ-TREE, RAxML]
    BI --> BI_Soft[e.g., MrBayes, BEAST]
