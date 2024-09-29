# LLM is all you need
Code for doing generation, extraction, prediction, retrieval, and evaluation tasks using LLMs. You can also find resources to start learning LLMs and use these codes as training material. 

### Introduction and aim 

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
  - ...loading
  
- Prediction
  - ...loading
  
- Retrieval and Retrival Augmented Generation (RAG, which is super cool)
  - ...loading
 
- Evaluation (LLM-as-a-judge)
  - ...loading

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

------
# Reousrces for learning
### Start
I really like learning projects by doing them. My suggestion is to put 1 week for learning (if you know Python) and then dive into a project. But people learn differently and they should consider their learning style, so here are resources you can use: 
- If you want to first learn and then do projects:
   - & You like youtube: 
      - YT playlist covering all aspects, from beginner-level to advanced: [Generative AI by Washington Prof](https://www.youtube.com/playlist?list=PLjy4p-07OYzui0nVZzMgoLBeXjG9Oy3hi)
    - & you like books:
      - A book covering all aspects of LLMs (really a great book, the second book I tried to read cover-to-cover in my life): [Hands-on Large Language Models by J. Alammar](https://www.amazon.co.uk/Hands-Large-Language-Models-Understanding/dp/1098150961/ref=asc_df_1098150961/?tag=googshopuk-21&linkCode=df0&hvadid=696285193871&hvpos=&hvnetw=g&hvrand=1585991372394813751&hvpone=&hvptwo=&hvqmt=&hvdev=c&hvdvcmdl=&hvlocint=&hvlocphy=9222618&hvtargid=pla-2281435176658&psc=1&mcid=eb08b758a9b13e57a4825f7bcdbd46b4&th=1&psc=1&hvocijid=1585991372394813751-1098150961-&hvexpln=74&gad_source=1)
    - & like gamification:
        - Datacamp: [Theory](https://www.datacamp.com/courses/large-language-models-llms-concepts) + [Intor to LLMs Python](https://www.datacamp.com/courses/introduction-to-llms-in-python) + [Langchain and RAG](https://www.datacamp.com/courses/developing-llm-applications-with-langchain)

- If you like to learn fast and do projects:
  - [YT playlist with fast introduction and projects](https://www.youtube.com/playlist?list=PLqZXAkvF1bPNQER9mLmDbntNfSpzdDIU5)
 
### Advanced
If you finished your first project and want to go deeper:
- [Learn the fundamentals of generative AI for real-world applications by deeplearning.io](https://www.deeplearning.ai/courses/generative-ai-with-llms/)
- [Building systems with LLMs](https://www.coursera.org/projects/building-systems-with-the-chatgpt-api-project)


## Other stuff
Other good stuff:
- [Extraction with Pydantic: Using LangChain Output Parsers to get what you want out of LLMs](https://www.youtube.com/watch?v=UVn2NroKQCw&t=853s)
- [Step-by-step RAG project: chat with your PDF](https://www.youtube.com/watch?v=dXxQ0LR-3Hg)
- [Building Production-Ready Apps with Large Language Models ](https://www.coursera.org/learn/building-production-ready-apps-with-large-language-models)

## Best papers you should read
- Holistic Evaluation of Large Language Models

## Best sources you should visit
- [Github repo: LLM-course](https://github.com/mlabonne/llm-course)
