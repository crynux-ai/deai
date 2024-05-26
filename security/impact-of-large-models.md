# Impact of Large Models

The extraordinary capabilities of Large Language Models (LLMs) render them even more susceptible to the aforementioned attacks. Owing to their enhanced capacity, identifying malicious data becomes more challenging since the model's performance on evaluated tasks remains largely unaffected, even after the introduction of malicious data. Consequently, backdoor attacks, particularly data poisoning attacks, become significantly easier to execute, allowing malicious actors to manipulate LLMs into generating desired outputs with specific triggers.

The success of backdoor attacks implies that the model possesses spare learning capacity. In addition to the defense techniques mentioned earlier, LLMs can utilize fine-tuning to overwrite neurons tuned for backdoor inputs or prune these neurons to effectively mitigate the impact of backdoor attacks.
