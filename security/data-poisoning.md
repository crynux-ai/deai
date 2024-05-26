# Data Poisoning

Data poisoning involves introducing malicious data to manipulate model outputs towards the attacker's intention. It's effective in both general machine learning and federated learning. In DeAI environments, where data is provided by individuals, it's particularly vulnerable to such attacks.

For classification models, a prevalent technique in data poisoning is label-flipping, wherein honest training examples are systematically switched from one class label to another. Consequently, the affected model erroneously predicts these examples to the corresponding altered labels.

To defend data poisoning, several defense strategies have been proposed. Reject on Negative Impact (RONI) measures the impact of each training example on the error rate, and remove those with large nagatvie impact. Additionally, loss functions can be leveraged to detect and mitigate the influence of malicious data.

Data sanitization techniques offer another avenue for early identification of malicious data. Methods such as BERT embedding, activations analysis and provenance information analysis can aid in this detection process.
