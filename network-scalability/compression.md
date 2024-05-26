# Compression

Model compression\cite{han2015deep, choudhary2020comprehensive} reduces the size of models to reduce the size of model, thereby facilitating efficient communication of model weights or gradients\cite{lin2017deep}.

Quantization emerges as a prominent approach, wherein weights are quantized to lower bit precision\cite{hubara2016binarized}. This not only reduces model size but also enhances computational efficiency. Notable examples include DoReFa-Net\cite{zhou2016dorefa}, which employs 1-bit weights with 2-bit gradients .

Sparsification techniques focus on pruning weights with negligible impact on model performance, thereby reducing model capacity without significant loss in accuracy\cite{zhu2017prune}. In distributed training scenarios, only gradients surpassing a threshold are communicated, leading to 99% savings in gradient exchange\cite{aji2017sparse}.

Federated Dropout\cite{caldas2018expanding} trains and updates smaller subnets of the model, thereby reducing both local computation costs and communication payloads in federated learning.

Furthermore, factorization techniques offer a means to decompose weight matrices into low-rank representations, thereby reducing the bandwidth required for communication\cite{wang2018atomo}.

These diverse strategies collectively contribute to optimizing model communication in decentralized settings.
