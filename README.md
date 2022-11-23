# Causal_literature_trend
The causal literature trend data&visualization for paper *Claim Causality with Clarity* preprint at [arXiv](???).

## Data 
The data used for visualization has been obtained from a [PubMed]( https://pubmed.ncbi.nlm.nih.gov/) search.

### 1. Searching criterias

All the data are stored in [data/raw](data/raw)

   1. causal literature: 

      ```(((causality OR causal) AND ((""0000""[Date - Publication] : ""2022""[Date - Publication]))```
   2. Causal clinical literature;

       ``` (((causality OR causal) AND (clinical)) ) AND ((""0000""[Date - Publication] : ""2022""[Date - Publication]))```
   3. Cuasal neurology literature;

      ```(((causality OR causal) AND (neurology)) ) AND ((""0000""[Date - Publication] : ""2022""[Date - Publication]))```
   4. Causal psychiatry literature;

      ```(((causality OR causal) AND (psychiatry)) ) AND ((""0000""[Date - Publication] : ""2022""[Date - Publication]))```
   5. Causal neuroimaging literature;

      ```(((causality OR causal) AND (neuro imaging)) ) AND ((""0000""[Date - Publication] : ""2022""[Date - Publication]))```

   6. Causal neuroscience literature (deprecated);

       ```(((causality OR causal) AND (neuroscience)) ) AND ((""0000""[Date - Publication] : ""2022""[Date - Publication]))```

   7. Causal imaging literature (deprecated);

      ``` (((causality OR causal) AND (imaging)) ) AND (("0000"[Date - Publication] : "2022"[Date - Publication]))```
    
### 2. Data selection rationale 

We decided to focus on clinical neuroscience and neuroimaging related research, thus "Causal neuroscience literature" (too broad) and "Causal imaging literature" (too broad). We merge all the query results in one file. In order to visualzie the cumulative distribution of papers published in causal literature, we sum up all the data before 1980 respectively for the data sparsity before 1980. The final data file [causal_literature_darta.csv](data/causal_literature_darta.csv) looks like:

| Year | Causal | Clinical | Neuroscience | Neurology | Psychiatry | Neuroimaging | Imaging
| :---: | :---: | :---: | :---: |:---: | :---: |:---: | :---: |
| 2022 | 299993 | 111413 | 11632 | 15859 | 8597 | 4073 | 30532
| 2021 | ... | ... | ... | ... | ... | ... | ... | ... |
| ... | ... | ... | ... | ... | ... | ... | ... | ... |