# 🩺 AI Doctor Assistant — Fine-Tuned LLaMA 8B

A specialized language model fine-tuned on medical reasoning data to provide accurate and explainable clinical answers using **Chain-of-Thought** prompts.

---
🔗 Download weights: [Hugging Face Model Repo](https://huggingface.co/khushiMalik3122/Medical_Ai_Assistance)

---

## 📦 Model Details

| Item               | Description                                 |
|--------------------|---------------------------------------------|
| Base Model         | `deepseek-ai/DeepSeek-R1-Distill-Llama-8B`    |
| Fine-Tuning Method | LoRA via [Unsloth](https://github.com/unslothai/unsloth) |
| Precision          | 4-bit QLoRA                                 |
| Max Seq Length     | 2048 tokens                                 |
| Frameworks         | Transformers, PEFT, Unsloth, Datasets       |
| Total Steps        | 60 (demo)                                   |
| Dataset Size       | 500 samples                                 |

---

## 📚 Dataset

- **Name**: [`FreedomIntelligence/medical-o1-reasoning-SFT`](https://huggingface.co/datasets/FreedomIntelligence/medical-o1-reasoning-SFT)
- **Content**:
  - `Question`: Clinical scenario
  - `Complex_CoT`: Chain-of-thought reasoning
  - `Response`: Final medical advice/answer

---

## 🧠 Prompt Format

### Question:
A 61-year-old woman reports urinary incontinence when coughing or sneezing.

### Response:
<think>
This is stress incontinence, which occurs when intra-abdominal pressure increases and the pelvic floor muscles are weak.
</think>
Stress urinary incontinence



---
