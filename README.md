# FakeNewsGuard - AI-Powered News Authenticity Detector
Advanced fake news detection system using BERT transformer models and deep learning. Built with PyTorch, Transformers, and Gradio for instant news verification.
<p align="center">
    <img src="image_resume_matching_demo.png" alt="demo-img"/>
</p>

# 🎯 What This Solves
- **Problem:**
  Misinformation spreads 6x faster than real news on social media. Manual fact-checking can't keep up.

- **Solution:** This system automatically
  - Classifies news articles as real/fake with 77% accuracy using BERT
  - Provides confidence scores and probability breakdowns
  - Processes articles in real-time (< 1 second per article)
  - Explains classification decisions with attention mechanisms Built on a curated dataset of          10,000+ verified news articles with ground truth labels.

# ⚡ Quick Demo

- **Run in Google Colab (recommended):**
  - Upload Fake_News_Detector.ipynb to Google Colab
  - Upload your True.csv and Fake.csv datasets
  - Run all cells - everything installs automatically
  - Get instant results with the interactive Gradio demo
Test with your own articles: Just paste any news text into the interface

# 📈 Performance Results
From the trained BERT model:
- **Classification Accuracy**
  - Algorithm: BERT-tiny with frozen layers + classification head
  - Validation Accuracy: 77.00%
  - Training Speed: 3 epochs, ~2 minutes total
  - Model Size: 17.8MB (mobile-friendly)

- **Processing Speed:**
  - 0.8 seconds per article classification
  - Batch processing: 1000+ articles in under 15 minutes
  - Real-time inference via Gradio interface

- **Memory Efficiency:**
  - Max sequence length: 128 tokens
  - Batch size: 16 (optimized for Colab)
  - RAM usage: <2GB during training
 
# 🚀 Production Extensions & Next Steps
 System is research-ready for:

- **1. Real-time Social Media Integration**
  - Connect to Twitter/Facebook APIs for live monitoring
  - Stream processing with Apache Kafka
  - Alert systems for viral misinformation

- **2. Advanced NLP Features**
  - Fine-tune BERT on domain-specific news data
  - Add multi-language support (100+ languages)
  - Implement stance detection and bias analysis
  - Source credibility scoring

  
