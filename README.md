# Sustainable Computing Taxonomy

This repository presents a formalized taxonomy for Sustainable Computing.
The description is structured around three interconnected parts:

- A [**problem**](./problem.yaml) that connects a computing system to some environmental threat or damage;
- A [**countermeasure**](./countermeasure.yaml) that aims to address that problem;
- Pieces of [**evidence**](./evidence.yaml) that either unveil the problem or validate the efficiency of the countermeasure.

> TODO: insert graphic here

The complete taxonomy is shown below and is accompanied by a [description of the various terms](./taxonomy-description.md).

Finally, the repository hosts a [curated list of research studies or projects](./studies/) that are described using the taxonomy.  

```yaml
Problem:
    Cause:
        Agent:
            Category:
                - End users
                - Policy makers
                - Designers
                - Engineers
                - ...
            State:
                - Uninformed
                - Unmotivated
                - Unaware
        Technology:
            Type: 
                - Hardware
                - Software
            Issue:
                - Bloated
                - Operated unsustainably
                - Short lifetime
                - High-footprint functionalities
                - High-footprint manufacturing
                - Stagnating
                - ... 
        Life-cycle phase: 
            - Design
            - Production
            - Deployment
            - Operation
            - Decommission
    Impact:
        Type:
            - Direct
            - Indirect
            - Systemic
        Life-cycle phase:
        Nature:
        
Countermeasure:
    Intervention:
        Agent: 
        Action:
            Domain:
                - Technological
                - Regulatory
                - Behavioral
            Sustainable Rs:
                - Rethink
                - Refuse
                - Reduce
                - Reuse
                - Repair
                - Recycle
                - Rot
        Life-cycle phase: 
        Temporality: 
    Impact:
        Type:
            - Direct
            - Indirect
            - Systemic
        Life-cycle phase: 
        Nature: 
    
Evidence:
    Data:
        - Observations 
        - Models 
    Metrics: 
    Approach:
        - Top-down
        - Bottom-up
        - Hybrid
    Reasoning:
        - Attributional
        - Consequential
        - Hybrid
    Boundaries:
```
