<img src="https://huggingface.co/aigeek0x0/radiantloom-support-assist-7b/resolve/main/radiantloom-support-assist.png" alt="Radiantloom Support Assist" width="800" style="margin-left:'auto' margin-right:'auto' display:'block'"/>

## Radiantloom Support Assist 7B
[Radiantloom Support Assist 7B](https://huggingface.co/aigeek0x0/radiantloom-support-assist-7b) is a support-assistant large language model fine-tuned from [Zephyr-7B-Beta](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta), over a custom-curated dataset of 3,000 support-assistant examples prepared by AI Geek Labs. The context lenght for the model is 4096 and it is licensed for commercial use.

## Intended Uses & Limitations
The radiantloom-support-assist-7b is meticulously fine-tuned to deliver optimal performance as a support assistant in customer-facing applications, specifically designed for use in help center chatbots. Its versatile functionality extends to various applications that require support conversation and retrieval augmented generation (RAG). This includes, but is not limited to, the development of AI bots tailored for B2B SaaS companies, e-commerce websites, corporate websites, and personal websites.

It is not a state-of-the-art generative language model and is not designed to perform competitively on general tasks with more modern model architectures or models subject to larger pretraining corpuses.

## Prompt Template

```
<|im_start|>system
You are a helpful assistant.<|im_end|>
<|im_start|>user
{user_message}<|im_end|>
<|im_start|>assistant
```


## Model Usage
We encourage you to try out this model using Google Colab.
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1z7YvgyYVPnOSml60yh0rIJKTC9uDbbLq?usp=sharing)

Here are a few example use cases. if we query the model with

```
<|im_start|>system
You work as a support assistant for AI Geek Labs, an AI research and development lab, handling inquiries and providing assistance through their website.

Use the following pieces of context to answer the user's questions. If you don't know the answer, don't make up an answer, just say you don't know.

<context>
Get AI-powered, Startup-fast: Build & Tune Your LLM MVPs with AI Geek Labs
Invent the future of your business with our cutting-edge AI research, development, and fine-tuning services. We're your AI playground.
Stop waiting, build! We turn your AI vision into reality, fast. From email assistants to code generation, we build MVPs with the latest AI frameworks \
like Langchain and OpenAI, helping small businesses and startups jumpstart their AI journey.
MVP: Turn your AI dream into a working prototype, lightning-fast. We design, develop, and deploy AI-powered MVPs using cutting-edge frameworks \
like Langchain, HuggingFace, and Llama-Index.
LLM Fine-tuning: Tap into the true potential of LLMs for your specific needs. We fine-tune models for email assistants, customer support chatbots, \
code generation, text-to-SQL, and more.
Open Source Radiance: We're passionate about sharing! Explore our Radiantloom series, featuring open-source LLM models fine-tuned by our experts, \
ready for you to build upon.
<context/><|im_end|>
<|im_start|>user
Question: What is AI Geek Labs?<|im_end|>
<|im_start|>assistant

```

the model will return

```
AI Geek Labs is a research and development laboratory focused on AI technology. They offer a range of services including building and tuning machine learning models, developing AI-powered applications, and providing open source resources. Their goal is to help clients achieve their AI goals quickly and efficiently, using the latest technologies and frameworks. Whether it's building a startup or improving existing systems, AI Geek Labs aims to provide innovative solutions tailored to their clients' needs. Their team is dedicated to staying at the forefront of AI technology and sharing their knowledge through open source resources and collaborations.

```

and if we query the model with

```
<|im_start|>system
You work as a support assistant for AI Geek Labs, an AI research and development lab, handling inquiries and providing assistance through their website.

Use the following pieces of context to answer the user's questions. If you don't know the answer, don't make up a answer, just say you don't know.

<context>
Get AI-powered, Startup-fast: Build & Tune Your LLM MVPs with AI Geek Labs
Invent the future of your business with our cutting-edge AI research, development, and fine-tuning services. We're your AI playground.
Stop waiting, build! We turn your AI vision into reality, fast. From email assistants to code generation, we build MVPs with the latest AI frameworks \
like Langchain and OpenAI, helping small businesses and startups jumpstart their AI journey.
MVP: Turn your AI dream into a working prototype, lightning-fast. We design, develop, and deploy AI-powered MVPs using cutting-edge frameworks \
like Langchain, HuggingFace, and Llama-Index.
LLM Fine-tuning: Tap into the true potential of LLMs for your specific needs. We fine-tune models for email assistants, customer support chatbots, \
code generation, text-to-SQL, and more.
Open Source Radiance: We're passionate about sharing! Explore our Radiantloom series, featuring open-source LLM models fine-tuned by our experts, \
ready for you to build upon.
<context/><|im_end|>
<|im_start|>user
Question: Which AI frameworks does AI Geek Labs use to build MVPs for clients?<|im_end|>
<|im_start|>assistant

```

the model will return

```
AI Geek Labs uses the latest AI frameworks such as Langchain, OpenAI, and Llama-Index to build MVPs for clients. These frameworks are designed to provide a comprehensive set of tools for developing and testing AI applications, making them ideal for building prototypical models quickly and efficiently. Additionally, these frameworks offer a wide range of features, including natural language processing, machine learning, and computer vision, which can be leveraged to create innovative and impactful solutions. If you have any specific questions about how these frameworks can benefit your project, feel free to ask!

```

## Evaluations
We are encouraged by the initial assessments conducted using the [LLM-as-a-Judge method](https://arxiv.org/abs/2306.05685), particularly with the utilization of GPT-4. Our ongoing efforts involve a more comprehensive evaluation of the model. As we progress, we will continue to provide updates on our findings and share the results on this platform.

## Ethical Considerations and Limitations
radiantloom-support-assist-7b can produce factually incorrect output, and should not be relied on to produce factually accurate information. Because of the limitations of the pretrained model and the finetuning datasets, it is possible that this model could generate lewd, biased or otherwise offensive outputs. Therefore, before deploying any applications of radiantloom-support-assist-7b, developers should perform safety testing.

## About Radiantloom
Radiantloom trains open-source large language models tailored for specific business tasks such as email assistance, customer support, and database operations.

Learn more about Radiantloom by visiting our [website](https://radiantloom.com). Follow us on Twitter at [Radiantloom](https://twitter.com/radiantloom) to gain early access to upcoming Radiantloom large language models.
