# Adaptive RL Defense Against Cryptographic Adversarial Attacks

This project presents an **Adaptive Reinforcement Learning (RL) Defense Framework** designed to protect Large Language Models (LLMs) against sophisticated **cryptographic adversarial attacks**. These attacks exploit vulnerabilities in LLMs by embedding malicious intent in prompts through various cryptographic techniques like Caesar ciphers, Morse code, and contextual manipulation.

## Key Features
- **Dynamic Decryption**: An RL agent trained using Proximal Policy Optimization (PPO) to detect and decode cryptographic adversarial prompts.
- **Cross-Model Robustness**: Evaluated on multiple LLM architectures (e.g., GPT-2, LLaMA, and Mistral) to ensure adaptability and effectiveness.
- **Efficiency Optimization**: Fine-tuned models using Low-Rank Adaptation (LoRA) and 4-bit quantization, reducing computational overhead while maintaining high defense rates.
- **Ethical Compliance**: Incorporates a reward system to penalize ethical violations and incentivize compliance.

## Results
- **Attack Success Rate (ASR)**: Reduced by 30%, mitigating the impact of cryptographic attacks.
- **Benign Success Rate (BSR)**: Achieved 96.8%, ensuring minimal disruption to normal queries.

## Methodology
1. **Reinforcement Learning Framework**:
    - Formulated as a Markov Decision Process (MDP) with states representing ciphered prompts and actions representing decoded tokens.
    - Rewards calculated based on decryption accuracy, ethical compliance, and efficiency.
2. **Training Pipeline**:
    - Diverse dataset of ciphered and base prompts.
    - Fine-tuned using PPO for adaptive learning.
3. **Inference Pipeline**:
    - Real-time detection and decoding of ciphered inputs.

## Ciphering Techniques Used
- Caesar Cipher
- Morse Code
- Self-Cipher
- Unicode Manipulation
- ASCII Transformation
- Contextual Manipulation

## Dataset
The dataset includes both base prompts and ciphered prompts encoded using various techniques. For details, refer to the [Dataset Preparation](#dataset) section in the documentation.

## Technologies Used
- **Languages**: Python
- **Frameworks**: PyTorch, Hugging Face, RLlib
- **Optimization**: LoRA, 4-bit Quantization
- **Algorithms**: Proximal Policy Optimization (PPO)
