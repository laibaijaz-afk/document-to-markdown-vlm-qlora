# document-to-markdown-vlm-qlora

## 🚀 Overview
This project focuses on converting document images into structured Markdown using a Vision Language Model (VLM) fine-tuned with QLoRA.

Traditional OCR systems extract plain text but fail to preserve document structure. This project addresses that limitation by generating semantically rich Markdown that retains headings, tables, lists, and layout.

## 🎯 Objectives
- Understand multimodal learning (vision + language)
- Fine-tune a pretrained VLM efficiently using QLoRA
- Convert document images into structured Markdown
- Evaluate model performance on unseen data


## 🧠 Model & Approach

### Vision Language Model (VLM)
We used a pretrained multimodal model capable of understanding both images and text.

### QLoRA Fine-Tuning
- 4-bit quantization for memory efficiency  
- Frozen base model weights  
- LoRA adapters for lightweight training  

This approach enables training on limited GPU resources while maintaining strong performance.


## 📊 Dataset

### Nougat Dataset
- Document images (research papers, reports, forms)
- Corresponding Markdown outputs
- Includes:
  - Headings
  - Tables
  - Lists
  - Equations (LaTeX)

The dataset helps the model learn document structure, not just text extraction.



## 🔄 Workflow

1. Dataset Exploration  
2. Data Preparation (ChatML format)  
3. Train/Validation Split  
4. QLoRA Fine-Tuning  
5. Markdown Generation  
6. Evaluation & Visualization  


## 📈 Results

### ✅ Strengths
- Preserves document hierarchy  
- Generates clean Markdown formatting  
- Handles structured text effectively  

### ⚠️ Limitations
- Struggles with complex tables  
- Sensitive to low-quality images  
- Occasional formatting inconsistencies  


## 🧪 Testing

The model was evaluated on:
- Training samples (seen data)  
- Unseen document images  

This helps measure both learning and generalization capability.

## 🌍 Applications

- Research paper digitization  
- Legal and business document processing  
- Knowledge base creation  
- Historical document preservation
- 

## 🧩 Key Learnings

- Multimodal models enable deeper understanding than OCR  
- QLoRA makes large model fine-tuning accessible  
- Data quality significantly impacts performance  
- Prompt design plays a critical role  


## 🚧 Challenges

- GPU memory constraints  
- Handling long sequences  
- Complex preprocessing  
- Evaluation without perfect metrics  

## 🔮 Future Work

- Improve table and equation handling  
- Train on larger datasets  
- Add post-processing for cleaner Markdown  
- Build a more advanced user interface  

## 📌 Conclusion

This project demonstrates how Vision Language Models combined with QLoRA can transform document understanding. It goes beyond traditional OCR by generating structured, meaningful Markdown output.

## ⭐ Acknowledgements

- Hugging Face Transformers  
- PyTorch  
- Kaggle GPU environment  
- Nougat Dataset  

## 📬 Feedback

Feel free to open an issue or share feedback!
