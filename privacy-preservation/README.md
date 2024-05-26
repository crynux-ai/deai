# Privacy Preservation

Privacy serves as a foundational principle in Decentralized AI (DeAI) systems. Data providers identify privacy leakage as their primary concern, highlighting the need for a trust mechanism to uphold their confidentiality in DeAI. The privacy preservation becomes more important in the context of handling powerful large models. These models, while offering increased capacity and capability, can become vulnerable to privacy leaks during inference due to their very nature.

Large language models demonstrate remarkable memorization capabilities and the capacity to learn from minimal data samples through techniques such as few-shot prompting. While this adaptability enables them to deliver impressive outcomes across various tasks, it simultaneously raises concerns regarding potential privacy breaches. The very nature of these models, with their vast parameter spaces and ability to internalize vast amounts of data, makes them susceptible to inadvertently disclosing sensitive user information during inference.

Moreover, the decentralized nature of AI exacerbates privacy risks. Traditional centralized models involve data being stored and processed in a single location, allowing for relatively easier implementation of privacy safeguards. In contrast, decentralized AI distributes data and computation across multiple nodes, complicating the task of ensuring privacy protection throughout the system.

Privacy attacks in DeAI systems can be categorized as follows:&#x20;

* &#x20;**Network data leakage**: Unique to DeAI, this leakage occurs when data is transmitted between computing nodes, posing challenges absent in centralized AI training or federated learning where data is located on computing power.
* **Membership inference attack(MIA)**: With this attack, adversaries predict if a specific example is part of the training data based on inference outputs
* **Training data extraction**: The superior memorization capability of large models renders them vulnerable to privacy leakage, particularly when personally identifiable information (PII) is included in training data. For instance, the study extractes training data containing PII such as names, phone numbers, email addresses, IRC conversations, code snippets, and 128-bit UUIDs from GPT-2 inference.
* **Gradient leakage**: Despite computation occurring on devices with data in federated learning, privacy can still be compromised as local training data can be reconstructed from gradients. TAG demonstrates the capability to reconstruct 88.9% tokens of private training data from gradient.
* **Attribute inference attack**: This attack infers personal attributes from text given at inference time. GPT-4 achieved 84% accuracy to predict users' personal attributes from their public posts in reddit.

In DeAI model training, data privacy preservation can be addressed in three stages:

* **Data Preprocess**: Techniques such as data filtering, noise introduction, anonymization, and data aggregation mitigate privacy risks locally before data transmission.
* **Computation Framework**: Privacy preservation can be ingrained within the design of the computation framework. Federated Learning, for example, aggregates user private data to train models while ensuring protection by locally computing gradients without revealing user data. Additionally, cryptographic computation methods like Multi-party computation (MPC), Homomorphic Encryption (HE), and Trusted Execution Environment (TEE) play a pivotal role in safeguarding user data privacy without divulging them to the computing nodes.
* **Model training**: Techniques like adversarial regularization, differential privacy, dropout, model stacking, and random deletion of neural connections enhance privacy during model training.



