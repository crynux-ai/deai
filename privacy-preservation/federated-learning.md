# Federated Learning

Federated Learning is a distributed machine learning paradigm that aggregates model gradients from decentralized data sources. In this paradigm, data providers compute gradients locally with a global model and local data, which are then shared with a coordinator. The coordinator manages the training process by distributing tasks to data providers and iteratively updating the model.

While traditionally the coordinator in federated learning is a centralized server, there are emerging studies exploring decentralized paradigms of serverless federated learning.

While federated learning stands as one of the most practical paradigms for preserving privacy in machine learning, it encounters several challenges:

* **Expensive Communication**: The iterative communication between devices and the server for model updates significantly increases communication costs, especially for large models.
* **Systems Heterogeneity**: Devices exhibit vast differences in storage capacity, computational power, communication bandwidth, and availability. With millions of devices in the network, this heterogeneity leads to high levels of unreliability.
* **Statistical Heterogeneity**: Data volume, quality, and distribution vary widely across different devices, presenting challenges in achieving consistent model performance.
* **Efficiency**: Compared to centralized model training, federated learning entails additional costs due to communication overhead and device unavailability, resulting in longer training times.
* **Privacy Concern**: Despite federated learning's emphasis on privacy preservation, there are instances of privacy issues arising from gradient leakage, which remain a concern&#x20;
