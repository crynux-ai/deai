# Copyright

Data providers within the DeAI paradigm may have concerns regarding the unauthorized utilization or potential plagiarism of their data by model trainers or other data contributors.

While ensuring privacy preservation necessitates defenses against membership inference and backdoor attacks, data providers are also interested in methods to detect if their data has been utilized in model training, particularly through the detection of specific triggers.

Data watermarking emerges as a prevalent technique applicable to various deep learning frameworks, including federated learning and LLMs. Among these techniques, intentional backdoor insertion stands out as a practical approach for data copyright detection, involving the introduction of noise or specific text as triggers, subsequently verifying the output embeddings for data ownership validation.
