# Zero-Knowledge Proof

Zero-Knowledge Proof (ZKP) is a cryptographic technique enabling a prover to convince a verifier of a statement's truth without revealing any additional information beyond the validity of the statement itself.

One prominent instantiation of ZKP is zk-SNARKs (Zero-Knowledge Succinct Non-interactive ARgument of Knowledge), which has been applied in machine learning domains. This novel paradigm facilitates the verification of AI computations, particularly in deep learning model inference scenarios, enabling computation offloading to untrusted devices while ensuring the integrity of the process.

However, in ZKP solutions, the translation of functions into arithmetic circuits entails high costs for proof generation. These costs can be as much as 1000 times greater than native computations, rendering ZKP solutions impractical for handling large models.
