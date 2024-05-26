# Model Poisoning

Model poisoning manipulates the global model by injecting malicious updates. It's a type of backdoor attack that maintains model performance on evaluated tasks but is controlled by attackers on backdoor tasks. Federated learning is vulnerable to model poisoning attacks, due to the decentralized nature of its participants, wherein any participant can update their model with injected malicious behavior

To address these risks, various defense methods have been proposed, primarily focusing on Byzantine robust aggregation techniques:&#x20;

* **Distance based methods**: These techniques distinguish outliers based on their distance from other agents.
* **Performance based methods**: These approaches evaluate updates and lower the weight of poorly performed updates.
* **Statistics based methods:** Utilizing the statistics of updates to identify outliers is another strategy employed to mitigate model poisoning attacks.

These defense mechanisms aim to enhance the resilience of federated learning systems against model poisoning attacks by effectively identifying and mitigating the impact of malicious updates.
