# CoDiStory: AI-Powered Bilingual Storytelling Platform for Children


CoDiStory is an AI-powered tool that generates short bilingual (Arabic & English) stories for children to strengthen their lexical abilities and support early education.
---

## Project Workflow

![Workflow Diagram](images/Workflow.png)


**Demo Video:** ([https://your-demo-video-link.com](https://youtu.be/a2YGLkdhBWs))  
---

## Example of a Generated Story

![Generated Story Example](path/to/generated-story-image.png)

---


## Overview

**CoDiStory** is an end-to-end AI pipeline that:
- Generates short stories from a single keyword using **LLaMA 2 + LoRA** fine-tuning.  
- Produces Pixar-style illustrations via **Stable Diffusion (DreamBooth + Textual Inversion)**.  
- Uses **Gemini 1.5 Flash** to transform each story scene into detailed image prompts.  
- Maintains character and style consistency across scenes.  
- Supports Arabic and English story output.

---

## System Architecture

1. **Text Generation Module (LLaMA 2 + LoRA)**  
   - Input: child’s name, gender, and target word  
   - Output: a 3–5 scene story  

2. **Prompt Generation (Gemini API)**  
   - Converts story scenes into detailed image prompts.  

3. **Image Generation (Stable Diffusion v1.5 + DreamBooth + Textual Inversion)**  
   - Produces Pixar-style images for each scene.  

4. **Frontend / Deployment**  
   - Multi-page **Flask or FastAPI Web App** with Firebase integration.  
   - Deployed in **Google Colab** or **local Jupyter environment**.  

---

## Hugging Face Model Links

| Token | Description | Embedding names in hugging face |
|--------|--------------|------|
| `<stylii>` | Pixar-style embedding | `LeenSMN/deployingEmbeddings`|
| `<wucs>` | Boy character embedding | `LeenSMN/deployingWindUp_200Steps` |
| `<lbcs>` | Girl character embedding | `LeenSMN/deployingLuca_400Steps` |


## Acknowledgment

This project was developed as part of our **Graduation Project** at  
**The University of Jordan – King Abdullah II School of Information Technology**  
**Department of Artificial Intelligence**

Supervised by: **Dr. Omar Alkadi**  
Domain Expert: **Miss. Salma Abdeljaber**

We sincerely thank our supervisor and domain expert for their continuous support, valuable guidance, and encouragement throughout the development of this project.

---

## Team Members

| Name | Role |
|------|------|
| **Beesan Al-Attal** | character consistency through scenes |
| **Layan Balbisi** | fine tuning LLM and generating story text|
| **Leen Samman** | style consistency |
| **Zaina Abu-Naser** | Frontend and Deployment |

---

