# Consensus Protocol

Consensus protocols utilize smart contracts to orchestrate verification workflows while distributing AI computations across decentralized devices. Crynux H-net\cite{crynux2023hnet} establishes a permissionless and serverless DeAI network, and verifies computation results by cross-validating with other nodes executing the same task. This approach involves two key steps: \begin{enumerate} \item Nodes upload commitments, derived from hashed signatures of results using local private seeds, onto the blockchain. \item Following the submission of commitments by all nodes, they can then submit their results to the blockchain for verification by smart contracts. \end{enumerate}

This consensus protocol effectively circumvents collusion among nodes, eschews reliance on trusted validators, and avoids additional computation complexity, rendering it well-suited for handling large models in DeAI settings.
