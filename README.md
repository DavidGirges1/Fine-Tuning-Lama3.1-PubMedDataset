# 🧠 Fine-Tuning LLaMA 3.1 on PubMedQA Dataset

This exploratory project was created to satisfy a simple curiosity:  
**Can a general-purpose Large Language Model (LLM) like Meta’s LLaMA 3.1 8B be effectively fine-tuned on a local, domain-specific dataset?**  
The goal is to adapt the model for **medical question answering** using the [PubMedQA](https://huggingface.co/datasets/pubmed_qa) dataset and observe how it performs in specialized biomedical contexts.

---

## 🔬 Project Overview

This notebook outlines the end-to-end process of fine-tuning the **Meta LLaMA 3.1 8B** model using **LoRA (Low-Rank Adaptation)** on the **PubMedQA** dataset.  
The ultimate goal: leverage a powerful LLM for accurate, domain-specific medical Q&A tasks.

---

## 📚 Key Resources

- 📘 [PubMedQA Dataset on Hugging Face](https://huggingface.co/datasets/pubmed_qa)  
- 🐑 [Unsloth – Efficient LLaMA Fine-Tuning Library](https://github.com/unslothai/unsloth)  
- 📄 *Fine-Tuning Lama 3.1 Instruct Template (from GEMINI 2.5 Pro)*  

---
## 🚀 Training Method: LoRA Fine-Tuning

The fine-tuning approach used is **LoRA**, a parameter-efficient technique that enables adapting large models with minimal training cost. Instead of retraining all model parameters, LoRA injects trainable low-rank matrices into the transformer layers.

Key advantages:
- ⚡ **Reduced memory usage**
- 📉 **Faster training**
- 💾 **GPU-friendly on consumer hardware**

> Fine-tuning was conducted using the [Unsloth](https://github.com/unslothai/unsloth) library, known for its fast and memory-efficient LLaMA training.

---

## 📊 Dataset: PubMedQA

[PubMedQA](https://huggingface.co/datasets/pubmed_qa) is a benchmark biomedical question answering dataset composed of:
- Clinical yes/no/maybe questions
- Contextual abstracts from PubMed articles
- Expert-annotated answers

It provides an excellent test bed for evaluating how well LLMs can reason in the medical domain.

---

## ✨ Highlights

- 🩺 **Domain Adaptation**: Specializes a general LLM for biomedical QA tasks  
- ⚙️ **Efficient Training**: Uses LoRA for memory-efficient fine-tuning  
- 🔎 **Exploratory Scope**: A hands-on dive into the real-world process of adapting LLMs to local data  
- 🧰 **Ecosystem Integration**: Combines Hugging Face datasets, Unsloth, and instruction-tuning methods  

---

## 👨‍💻 Crafted By

**David E. Girges**  

---

## 🧪 Disclaimer

This project is for *experimental purposes only**.  
The fine-tuned model is **not intended for real medical advice or clinical use**.

