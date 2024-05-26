# Privacy Preserved Training

### Differential privacy

Differential privacy, defined as ensuring that adjacent data cannot be distinguished, offers privacy protection through an information-theoretic guarantee. In practice, differential privacy is implemented by adding noise to data, gradients, output, or objective functions. However, while differential privacy is crucial for preserving privacy, it may blur long-tail examples in data distributions, resulting in reduced accuracy, particularly for underrepresented groups. Despite its potential negative impact on pretrained model performance, differential privacy in fine-tune tasks can maintain model utility.

### Privacy Regularization

Privacy regularization introduces penalties for generating privacy-sensitive information. For instance, PPLM introduces instruction tuning with Direct Preference Optimization (DPO) to reward generations that distinguish between publicly shareable and privacy-sensitive information.
