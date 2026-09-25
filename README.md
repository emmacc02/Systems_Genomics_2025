# Systems_Genomics_2025

## PROJECT DESCRIPTION 
Pipeline for analysing RNASeq raw data from [Krausgruber et al. (2020)](https://www.nature.com/articles/s41586-020-2424-4) [1]

Dataset considered was specifically limited to samples in the control and LMCV-infected endothelial cells in the liver and the brain 

## GENERAL WORKFLOW
```mermaid
flowchart LR
    %% 1. Define Subgraph A (Keeps TB layout)
    subgraph A [Step 1: Prep Work]
        direction TB
        A1[Gather requirements] --> A2[Set up environment]
    end

    %% 2. Define Subgraph B (Keeps TB layout)
    subgraph B [Step 2: Database Migration]
        direction TB
        B1[Backup data] --> B2[Run schema scripts]
    end

    %% 3. LINK THE SUBGRAPHS GENERALLY (Do not link A2 to B1 directly)
    A --> B
    B --> C[Step 3: Deploy Application]
```

## REFERENCES 
[1] Krausgruber, T., Fortelny, N., Fife-Gernedl, V. et al. Structural cells are key regulators of organ-specific immune responses. Nature 583, 296–302 (2020). https://doi.org/10.1038/s41586-020-2424-4
