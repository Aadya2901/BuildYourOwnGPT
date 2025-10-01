# 🚀 Day 14 of 21 Days, 21 Projects Challenge  
📌 **Build Your Own GPT – Custom Text Generation Engine** ✍️📚  

---

## 🔎 Project Overview  
This project focused on training a **compact GPT-style model** on the **TinyStories dataset** to generate short children’s stories.  
Additionally, I implemented **prompt filtering** so that the model only responds to **Python coding queries**, returning a default message for others.  

---

## ⚙️ Tech Stack & Setup  
- **Frameworks:** PyTorch, Hugging Face Transformers  
- **Model Architecture:** GPT-2 style (`GPT2LMHeadModel`)  
- **Dataset:** [roneneldan/TinyStories](https://huggingface.co/datasets/roneneldan/TinyStories)  
- **Optimizer:** AdamW with checkpointing for reproducibility  
- **Tokenizer:** Custom tokenizer for small-context modeling  

---

## 📊 Implementation Highlights  
1. Loaded and tokenized the TinyStories dataset  
2. Configured a **GPT-2 style architecture** for training  
3. Used **AdamW optimizer** + reproducible random seeds  
4. Added **checkpoint saving** for stable retraining  
5. Implemented **prompt filtering logic**:  
   - Responds to **Python coding prompts**  
   - Returns a default message for all other prompts  

---

## 🖼️ Observations & Results  
- The model generated **coherent and creative short stories** despite being trained on a small dataset  
- **Prompt filtering** helped restrict outputs to relevant use cases  
- The setup demonstrated that **compact LLMs can still achieve practical results** with the right controls  

---

## ✅ Key Takeaways  
- Even **small GPT models** can generate useful outputs with careful training  
- **Reproducibility (seeds + checkpoints)** ensures stable experimentation  
- **Custom filtering** adds practical guardrails to text generation  

---

## 🔮 Future Work  
- Fine-tune on additional datasets (e.g., fairy tales, code snippets)  
- Experiment with **quantization** for deployment on edge devices  
- Add **classification-based filtering** instead of keyword matching  

---

## 📂 Repository Contents  
- `TinyStories_GPT.ipynb` → Training & evaluation notebook  
- `results/` → Generated samples and metrics  

---

## ⚡ References  
- [Hugging Face Transformers Documentation](https://huggingface.co/docs/transformers/index)  
- [TinyStories Dataset](https://huggingface.co/datasets/roneneldan/TinyStories)  
- [PyTorch Documentation](https://pytorch.org/docs/stable/index.html)  
