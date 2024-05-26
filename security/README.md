# Security

Malicious actors within DeAI environments pose significant privacy and security concerns. While malicious computing nodes and training tasks can leak the privacy of data providers, malicious data providers may compromise the security of DeAI models. Attacks targeting models and federated learning can both impact DeAI systems by reducing model quality or inducing models to output desired contents.

DeAI involves permissionless participants in the network, making it vulnerable to network attacks. Common attack means from the perspective of network participants include:&#x20;

* **Byzantine attack**: Malicious agents upload arbitrary updates to degrade training performance.
* **Sybil attack**: Attackers create multiple dummy participant accounts to gain larger influence.&#x20;

In DeAI, attackers often focus on the model during its training or inference phases, aiming for either targeted or untargeted poisoning. Targeted poisoning involves attackers manipulating the model to produce desired outputs of their choosing. On the other hand, untargeted poisoning seeks to disrupt the convergence of the global model, diminish its accuracy, or even cause it to diverge from its intended behavior. Data poisoning and model poisoning are common methods employed by attackers to achieve these objectives.
