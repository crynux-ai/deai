# Challenges

Each privacy preservation approach has its drawbacks. Cryptographic methods guarantee a high level of privacy but suffer from significant efficiency drawbacks and may not defend against membership inference attacks. Differential privacy and adversarial regularization mitigate privacy attacks to some degree without introducing additional computation costs but may impact model performance. These challenges are often mutually incompatible. Furthermore, the strengths of these techniques can also be double-edged; cryptographic approaches prevent data leakage in communication but also hinder data auditing, potentially facilitating backdoor attacks and data poisoning. To mitigate these challenges, multiple techniques are often used together, with federated learning serving as a backbone to integrate with other techniques such as differential privacy, MPC, and cryptographic methods. Some studies introduce trusted third parties to address efficiency challenges.



| Method | Model Performance | Efficiency      | Network Requirement | Risk             |
| ------ | ----------------- | --------------- | ------------------- | ---------------- |
| DP     | Lower             | Similar         | Low                 |                  |
| FL     | Similar           | Sligntly slower | High                | Gradient leakage |
| FHE    | Much lower        | Much slower     | Low                 | MIA              |
| TEE    | Same              | Much slower     | Low                 | MIA              |
| MPC    | Same              | Much slower     | Very high           | MIA              |

