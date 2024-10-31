
### Intro

This repo contains code for doing generation, extraction, prediction, retrieval, and evaluation tasks using LLMs. You can also find resources to start learning LLMs and use these codes as training material. 


The project's code is structured considering how you may want to use LLMs, instead of nesting codes for each project next to each other. This will help you to find the code you want faster. I also provided some examples that you can play with to test the code. 

- Generation   _...loading_
  - OpenAI API
  - Claude API
  - LM studio server (local models, the painless way)
  - Ollama (local models, the hard way)
  - Groq (cloud server for running popular open-source LLMs)
  - Poe (Poe is UI to play with many LLMs without hosting them locally. You can play a trick to get the answers automatically)
  - HuggingFace API (cloud server for running almost all open-source LLMs)


- Extraction
  - [EXCT_GIANT](https://github.com/Nadkarni-Lab/GIANT/tree/main/EXCT_GIANT): Langchain + asyncOpenAI + Pydantic --> Multi-level dictionary with painless error handling for parser 
  
- Prediction
  - ...loading
  
- Retrieval and Retrival Augmented Generation (RAG, which is super cool)
  - ...loading
 
- Evaluation (LLM-as-a-judge)
  - ...loading
 
- Multimodal:
  - [TiLense](https://github.com/Sdamirsa/TiLense-4BlackBox-VLM): OpenAI-Vision + Prediction (Function Call) + Tile-based Masking --> An explainability module (tile importance for prediction task) for black-box vision language models 

Before pushing the code into this repo, I tried my best to clean it, make it modular, and add code guides to make it reusable. The codes in this repo are part of my projects named:

- **LLManswerGIBoard**: Asking multiple local, commercial, and quantized LLMs to answer GI board single best answer MCQ. A benchmarking study with the generation of answers and semi-automated evaluation. 
- **EXAMINER**: A tool that generates standardized questions using the provided document. This is a RAG-based open-source project.
- **Merge-Guidline-Tool**: merging multiple medical guidelines from different associations with similar topics into one document with merged outline, similarity, dissimilarity, and final statements for each section. This is a RAG-based open-source project.
- **LLMvsCML-COVID19**: Comparison of LLMs with classical machine learning models on prediction of COVID-19 in-hospital mortality. This is a prediction task we tackled using generation, along with fine-tuning a small LLM.
- **LLMvsCML-PolypImage**: Comparison of Vision LLMs with machine learning models on polyp detection and classification in colonoscopy images. This is a prediction task we tackled using generation, along with the code for fine-tuning CLIP.
- **GI-Copilot**: A chatbot that answers your questions using validated sources (guidelines published by five GI associations). This is a RAG-based project.
- **EXCT**: Extraction of information from MR enterography report and then use them for calculation of a severity score. This is an extraction project.

### Consideration for use 

- **My context**:
I am using a dual boot (Linux and) Windows-based laptop with RTX3080Ti (16GB graphic memory) and Core-i9 (12900HX). I am using Visual Studio Code, notebooks, and my local processor for anything I do (no Colab or Kaggle). 

- **Changes in libaries**:
The rapid development of LLMs and their libraries makes codes less reusable. I started playing with langchain and llama.index using their 0.1 version. I'll try to update the old ones, but if you got into a problem running any of them, open an issue. 

- **Challenging setup (especially when you want to use your GPU)**:
Setting up the environment and installing the libraries correctly may become challenging if you want to use GPU. If you want to use any local LLM, start by having an LM studio server, which is painless. 

- **easy yet difficult to imitate**:
Using LLMs is "easy yet difficult to imitate." While you may think that using these tools is super easy and adaptable for any use case, you should have a testing stage to find the best approach and parameters for your use case. So, don't overlook the impact of LLM setup and design to do your task. You should probably hard code your own solution, while using examples can help you to boost your speed. 
