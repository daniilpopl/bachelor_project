# Exploring Large Language Model for Hate-Speech Meme Detection

## Daniil Paplauski
Vrije Universiteit, The Netherlands

### Overview
This project explores the application of large language models (LLMs) for detecting hate speech in memes.

### Table of Contents
1. [Problem and Motivation](#problem-and-motivation)
2. [Description and Justification of Research Approach](#description-and-approach)
3. [Experimental Setup](#experimental-setup)
4. [Results](#results)

### Problem and Motivation
This research aims to explore the use of prompt engineering to enhance LLMs' ability to accurately detect hate speech in memes.
This study addresses two main research questions:
1. How do various prompting techniques influence hate speech detection?
2. How does OCR-extracted text influence the results?

### Description and Approach
The research focuses on different prompting strategies for hate speech detection in memes. 
It uses the BLIP model for image captioning and Tesseract for OCR to extract text from images. 
The study compares the proposed framework with related models, including Concat BERT, Visual BERT COCO, CLIP, Hate-CLIPper, and Fuser-HMC.

### Experimental Setup
The experimental setup involves several steps:
1. **Data Preparation:** Using the Facebook Hateful Memes dataset.
2. **Image Processing:** Enhancing images for text extraction using bilateral filtering, grayscale conversion, and thresholding.
3. **Image Captioning:** Generating captions for each image using the BLIP model.
4. **Prompt Generation:** Constructing prompts using predefined strategies.
5. **Meme Analysis:** Classifying memes as hateful or not using the OpenAI GPT-4o model.
6. **Evaluation:** Assessing performance using accuracy and AUROC metrics.

### Results
Direct prompts showed the best performance, achieving an accuracy of 0.70. However, fine-tuned models like Hate-CLIPper outperformed LLMs.
Use of OCR text instead of annotated one leads to average 4% perfomance reduction.
