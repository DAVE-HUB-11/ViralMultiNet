# ViralMultiNet: A Structure-Aware Multimodal Framework for Viral Genome Classification

> **📢 Manuscript Under Review**
> 
> This repository contains the official implementation of **"ViralMultiNet: A Structure-Aware Multimodal Framework for Viral Genome Classification"**, currently under review at *BMC Bioinformatics*.

## 🚀 Overview

ViralMultiNet is a novel multimodal deep learning framework that integrates multi-scale viral DNA sequences with functional annotation texts through structure-aware attention and cross-modal knowledge distillation for robust viral genome classification.

1. K-mer Tokenizer Files
   - Directories: tokenizer_[4/5/6/7]mer/
   - Contents per directory:
     * vocab.txt (token vocabulary)
     * config.json (tokenization rules)
     * special_tokens.json (boundary tokens)
   - Usage: ViralDNA sequence segmentation

2. Annotation Embedding Files
   - Files: anno_embs_{train/val/test}.npy
   - Format: NumPy array (float32)
   - Description: Precomputed UniProt FUNCTION field embeddings

3. Dataset Samples (100-row subsets)
   - Files: dataset_balanced_{train/val/test}_head100.xlsx
   - Ethical Compliance: No identifiable metadata (IRB exempt #GXU-2024-BIO01)
   - Note: Full dataset (1.39 GB) available upon request

4. High-Attention Motifs
   - Files: high_attention_kmers_branch{0..3}_clean.fasta
   - Analysis Tool: MEME Suite v5.5.5 (http://meme-suite.org)
   - Validation: JASPAR 2024 results in Table S3

5. Pretrained Model Weights
   - File: pretrained_multiscale_bert.pt
   - Version: ViralBERT-v1.0 (PyTorch 2.1.0+cu121)
   -

---

Access Notes
- Total Supplement Size: 4.2 GB (compressed .zip)
- Request Full Data: Email lgdzhy@126.com with institutional affiliation
- Reviewer Access: Pre-authorized via ScholarOne system


## 📋 Requirements

```bash
pip install -r requirements.txt