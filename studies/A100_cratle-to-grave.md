---
Problem:
    Cause:
        Agent:
            Category:
                - Policy makers
                - Procurement Engineers
            State:
                - Uninformed
        Technology:
            Type: 
                - Hardware
            Issue:
                - High-footprint functionalities
                - High-footprint manufacturing
        Life-cycle phase: 
            - Design
            - Production
            - Deployment
            - Operation
            - Decommission
    Impact:
        Type:
            - Direct
        Life-cycle phase: 
            - Design
            - Production
            - Deployment
            - Operation
            - Decommission
        Nature: GPUs that are extensively used for AI applications have a large environmental footprint, not just in GWP, but in most of the 16 impact vectors identified in the LCA standard.
        
Evidence:
    Data:
        - Observations 
    Metrics: 
    Angle:
        - Bottom-up
    Reasoning:
        - Attributional
    Boundaries:
        - A single GPU card
    
Countermeasure: None
---

Interesting paper that tears down a GPU card (A100) to get a precise estimate of the material composition (primary data) rather than relying on secondary data (activity estimates from LCA databases).

If shows that the climate change impact is relatively well estimated in the existing databases, but others impact factors, much less so.

It continues to assess the impact of the activity of training GPT-4 and BLOOM. Unsurprisingly, the operational impact strongly dominates most of the environmental impacts (climate change in particular) but manufacturing still dominates some key impacts: human toxicity, cancer (99%), eco-toxicity, freshwater (37%) and mineral and metal depletion (85%).

Another interesting data point is the normalization of the training impact of LLMs by with a Planetary Boundary (PB)-aware normalization method (Sala et al (2018) [45]).
