# Literature Review

Approaches or solutions that have been tried before on similar projects.

**Summary of Each Work**:

- **Source 1**: Zephyr-7B: Fine-tuning and Inference with W&B

  - **[Link](https://wandb.ai/vincenttu/finetuning_zephyr7b/reports/Zephyr-7B-Fine-tuning-and-Inference-with-W-B--Vmlldzo1ODc0MTcx)**
  - **Objective**: Explains how Zephyr-7B model is fine-tuned based on the Mistral-7B model and provides an example on how to fine-tune it with Weights & Biase.
  - **Methods**: Utilizes Hugging Face and W&B to fine-tune the Zephyr-7B on the a dataset with 1,866 chat interactions for chatbots as agents ("AgentInstruct" dataset).
  - **Outcomes**: Demonstrates how to fine-tune (SFT only) Zephyr-7B on AgentInstruct. Uses W&B Tables to track model inputs and outputs. Provides full notebook and hyper-parameter settings for fine-tuning and inference.
  - **Relation to the Project**: It uses comparable model fine-tuning techniques, however, focusing on improving agent abilities in LLMs and not educational helpfulness.

- **Source 2**: Fine-tuning Mistral 7B with W&B

  - **[Link](https://wandb.ai/vincenttu/finetuning_mistral7b/reports/Fine-tuning-Mistral-7B-with-W-B--Vmlldzo1NTc3MjMy)**
  - **Objective**: Explains how Mistral-7B is fine-tuned on a single GPU (T4).
  - **Methods**: Utilizes Hugging Face and W&B to fine-tune a Mistral 7B on the Puffin dataset, 3000 multi-turn conversations between a user and GPT-4.
  - **Outcomes**: Demonstrates how to fine-tune (SFT only) Mistral-7B on the Puffin dataset. Uses W&B Tables to track model inputs and outputs. Provides full notebook and hyper-parameter settings for fine-tuning and inference.
  - **Relation to the Project**: It uses comparable model fine-tuning techniques, however, focusing on improving general model performance by data distilled from GPT-4 and not educational helpfulness.

- **Source 3**: Fine-tune Llama 2 with DPO

  - **[Link](https://huggingface.co/blog/dpo-trl)**
  - **Objective**: To fine-tune the Llama v2 7B-parameter model using Direct Preference Optimization (DPO), offering a simplified approach to aligning language models with human preferences without the complexity of traditional reinforcement learning.
  - **Methods**: The process includes supervised fine-tuning (SFT), using a dataset of preference annotated data with chosen and rejected responses, and then applying DPO training. This method bypasses the need for reward modeling and complex RL optimization, using TRL library tools like Peft and Accelerate for efficient training.
  - **Outcomes**: The successful implementation of DPO for fine-tuning Llama v2, demonstrated by improved reward metrics like higher chosen rewards over rejected ones. The training scripts and final model were made available, showcasing effective alignment of the model with human preferences.
  - **Relation to the Project**: DPO provides an alternative and simplified method for fine-tuning language models using RLHF on specific objectives like educational helpfulness.
