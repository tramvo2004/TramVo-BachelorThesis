# High-Value Target Detection & Enhanced ALE Calculation

## Project description

The process of this project contains two main parts. The first part focuses on evaluating the risk associated with each asset and accurately determining its value, recognizing that not all assets contribute equally to operational continuity. Based on the result from the first part, the second part involves calculating Annual Loss Expectancy (ALE), which aims to create a more precise estimation of the potential financial impact of cyber incidents. Probabilistic graphical models will be applied as they offer a structured and probabilistic approach to modelling the complex interdependencies among assets, vulnerabilities, and risk factors in (Operational Technology) OT environments. The research aims at testing the accuracy and feasibility of applying probabilistic graphical models, not only in detecting high-value assets but also in assessing assets’ value and expected loss.

## Research question 
To what extent do probabilistic graphical models accurately estimate asset value and expected loss based on network position?

## Key Metrics

- External‑attack probability ($p_j$): Likelihood that an asset is compromised from an external source.

- Internal‑exploit probability ($p_{ij}$): Likelihood of propagation between connected assets, assigned for each directed connection.
 
- BAG inference ($p_{base}$): Marginal compromise probabilities via noisy‑OR model.

- Cascade impact: Monte Carlo estimates of breach propagation starting from each asset.

- ALE computation: Asset Value (AV), Exposure Factor (EF), Single Loss Expectancy (SLE).

# Risk prioritization based on $p_{base}$
The red nodes are high-risk assets and the green nodes stand for low-risk assets
![image](https://github.com/user-attachments/assets/6950a61f-a867-4200-8181-5bcfcc5cff3c)
