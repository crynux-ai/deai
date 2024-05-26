# Parameter-Efficient Fine Tuning

Within the landscape of large-scale models, conventional compression techniques may prove insufficient to address the challenges posed by their large size. In this context, Parameter Efficient Fine Tuning (PEFT) emerges as a more aggressive strategy aimed at reducing the number of trainable weights, thereby mitigating communication overhead.

PEFT adjusts only a small proportion of model parameters, resulting in a significant reduction in computational complexity. This reduction in the number of trainable weights translates to a decrease in communication payload, particularly beneficial in Decentralized AI (DeAI) settings.

PEFT can be categorized into several approaches\cite{han2024parameter}:&#x20;

* Additive modules modifies the model architecture by injecting an additive trainable modules or layers \cite{houlsby2019parameter, pfeiffer2020adapterfusion}.
* Soft prompts utilize continuous embedding spaces of soft prompts to refine model performance. Notable examples include Prefix-Tuning, which leverages prefix vectors for inference after fine-tuning \cite{li2021prefix,liu2021p}.&#x20;
* Selective fine-tuning involves selecting a small subset of parameters, making them tunable while keeping the remaining weights frozen. Diff Pruning\cite{guo2020parameter,vucetic2022efficient} applies parameter pruning techniques to achieve efficiency gains . \item Reparameterized PEFT employs low-rank parameterization techniques to construct more efficient representations, which are then transformed back for inference\cite{hu2021lora}.

The emergence of large-scale models has catalyzed the development of diverse techniques aimed at significantly reducing the computational complexity and communication overhead associated with these models in the realm of DeAI.
