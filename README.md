# 🧠 Small Reasoning Model for GSM8K 🚀

![Math Reasoning](https://img.shields.io/badge/Math-Reasoning-blue)
![RL Training](https://img.shields.io/badge/RL-Training-green)
![GSM8K](https://img.shields.io/badge/Dataset-GSM8K-orange)

## 🔥 Supercharging Small Language Models with GRPO!

This repository showcases a cutting-edge implementation of **Group Relative Policy Optimization (GRPO)** to enhance the mathematical reasoning capabilities of compact language models on the challenging GSM8K dataset.

## 💡 What is GRPO?

**Group Relative Policy Optimization (GRPO)** (Shao et al., 2024) is an efficient reinforcement learning approach that:

- **Eliminates the need for a critic model** typically the same size as the policy model
- **Estimates baselines from group scores** instead of using a separate value network
- **Dramatically reduces training costs** while maintaining performance
- **Samples a group of outputs** {𝑜₁, 𝑜₂, ⋯, 𝑜ᴳ} from the old policy and optimizes based on relative performance

## ✨ Key Features

- **Multi-faceted Reward System** with five complementary components:
  - ✅ **Correctness rewards** for accurate solutions
  - 🔢 **Integer validation** ensuring numerical answers
  - 🏗️ **Format enforcement** (strict and soft) for XML structure
  - 🧩 **Granular XML rewards** with partial credit

- **Elegant Structured Output**:
  ```xml
  <reasoning>
  Step-by-step solution process
  </reasoning>
  <answer>
  Final numerical answer
  </answer>
  ```

- **LoRA Fine-tuning** for parameter-efficient updates

- **Model Flexibility** supporting both Llama-3.2-1B and Qwen2.5-1.5B architectures

## 🛠️ Implementation Highlights

- Leverages the **TRL library** for reinforcement learning
- Custom reward functions for **precision output formatting**
- **W&B integration** for experiment visualization
- **Flash Attention 2** for memory-efficient training
- Options for **few-shot learning** configurations

## 📊 Results

Our trained models show significant improvements in:
- Structure adherence with proper reasoning steps
- Answer accuracy on mathematical word problems
- Format consistency across varying problem complexity

## 📝 Acknowledgement
UNSLOTH and [@willccbb](https://gist.github.com/willccbb/4676755236bb08cab5f4e54a0475d6fb) for data prep and all reward functions.

## 🔮 Future Directions

Check out the [GitHub repository](https://github.com/willccbb/verifiers) for ongoing developments and new breakthroughs in small model reasoning capabilities.


---

### 🌟 Join the revolution of making small models reason like the big ones! 🌟
