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

## Approach in the project
The final report and code file follows similar outlines.

![Screenshot 2025-06-25 at 11 28 28](https://github.com/user-attachments/assets/6dc7b906-6aa9-4f92-ad81-6b59b49b11f3)
![Screenshot 2025-06-25 at 11 27 19](https://github.com/user-attachments/assets/f2d8bbee-e056-4144-9291-93c4aee600e3)
![Screenshot 2025-06-24 at 18 56 04](https://github.com/user-attachments/assets/a150c6cf-d2fa-4adb-916f-6683f71789f3)



## Experimental results

The experimental results were illustrated in the .ipynb files.

Main summary of the results:
1. $p_j$:
   - Identify the assets that more likely to be chosen as the initial attack point.
   - Highlight the asset categories that has higher chance of becoming a target.
2. $p_{ij}$
   - High-risk connections were identified with a threshold of 0.75.
   - Detect the group of assets that often involed in high-risk connections.
3. $p_{base}$: Risk prioritization for assets in the network.
4. mean_cascade and the chance that an asset spread the infection to at least one another asset if it is compromised.
   - Identify top critical assets, those with the ability to spread the infection to entire network.
   - Point out asset categories that have high impact on the network.
5. ALE: the influence between each components on ALE.
   
