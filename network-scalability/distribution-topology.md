# Distribution Topology

Many techniques derived from distributed computing are applied in DeAI settings, offering innovative solutions to various challenges.

Decentralized training exhibits potential advantages over centralized counterparts, particularly in scenarios characterized by network constraints such as low bandwidth or high latency\cite{lian2017can}.

Parallelism strategies are pivotal for accelerating model training across multiple GPUs, addressing the computational challenges inherent in large-scale models.

Data parallelism stands as the most prevalent approach, wherein datasets are partitioned into subsets and distributed among workers, each equipped with a model replica. Here, each worker processes a mini-batch within its assigned subset, computing weight updates independently. Communication is essential to synchronize gradients computed across devices. Parameter servers \cite{li2014scaling} and AllReduce communication protocols\cite{patarasuk2009bandwidth} facilitate this synchronization.

As large models nowadays exceed the capacity of a single GPU, model parallelism\cite{shoeybi2019megatron} emerges as a solution, distributing different parts of the model across multiple GPUs simultaneously.

Pipeline parallelism\cite{huang2019gpipe, narayanan2019pipedream} optimizes computation by breaking it into stages and forming a pipeline, with each stage executed on a distinct device. This method enhances throughput by enabling parallel processing of micro-batches.

These parallelism strategies relies on GPU interconnect techniques, such as NVLink and PCI-E \cite{li2019evaluating}. These techniques provide a high-bandwidth communication between GPUs that can be as high as 1000Gbps on a centralized server. However, the decentralized environment is built on internet with bandwidth of 10-100 Mbps.

Petal \cite{borzunov2022petals, borzunov2024distributed} allocates different layers of the model to decentralized GPUs on 10-100 Mbps internet for inference and infetune BLOOM-176B model\cite{le2023bloom}.

Studies are also made to pretrain and fine-tune foundation model on 500Mbps network\cite{yuan2022decentralized, wang2022fine}. They optimize scheduling based on a communication matrix incorporating bandwidth and latency information between decentralized nodes. Despite 100x slower communication, their distributed training setups across 64 GPUs in 8 regions globally incur only a 1.7-3.5x slowdown compared to centralized data centers.

In the federated learning context, hierarchical topology\cite{liu2019edge} is introduced to optimize communication efficiency of FL. This topology leverages edge servers to aggregate updates. This approach effectively reduces the overall communication burden.
