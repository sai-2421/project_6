# project_6
**GUVI GPT Model Deployment**

This project focuses on deploying a fine-tuned GPT model, specifically trained on GUVI's company data, using Hugging Face services. The deployed model is accessible via a scalable and secure web application built with either Streamlit or Gradio. Additionally, the application stores user login information (e.g., username and login time) in a database.

> **Objective**

The main goal is to deploy a pre-trained or fine-tuned GPT model using Hugging Face Spaces, making it publicly available through an easy-to-use web interface. The app can handle various use cases, such as customer support, content generation, educational assistance, and internal knowledge management.

> **Features**
- Customer Support Automation:

    Automates responses to frequently asked questions.
  
- Content Generation:

   Helps generate marketing content, such as blog posts or social media updates.
   
- Educational Assistance: 
  
   Acts as a virtual teaching assistant for students, answering queries related to course material.
    
- Internal Knowledge Base:

   Enables GUVI employees to quickly access internal documentation and information.
   
- Training and Onboarding:

   Assists in employee training by providing easy access to company resources and answering common questions.

> **Technologies Used**

- Hugging Face Transformers: For fine-tuning the GPT model.
  
- Streamlit or Gradio: For building the web application interface.
  
- Torch: For model training and inference.
  
- ngrok: For providing temporary public access (optional).
  
- Pyngrok: For tunneling local web apps (optional).
  
> **Business Use Cases**

- Customer Support Automation: Handles initial customer inquiries and common questions.
  
- Marketing Content Generation: Generates blog posts, social media content, and newsletters.
  
- Educational Assistance: Provides immediate answers to students’ queries.
  
- Internal Knowledge Base: Allows employees to query company-related data.
  
- Training and Onboarding: Facilitates new hires’ onboarding by offering instant access to relevant information.

> **Deployment on Hugging Face Spaces**
+ Upload your repository to Hugging Face Spaces.
  
+ Ensure all dependencies are listed in the requirements.txt file.
  
+ Follow Hugging Face’s documentation to configure and deploy the model.
  
> **Usage**

Once deployed, users can:

- Enter text prompts to interact with the GPT model.

- Access responses to queries or generate content based on the input.

- View user information such as login time.

  > **Packages and Libraries used**

```python  
# Run the Streamlit app and expose it via ngrok

from pyngrok import ngrok

# Import the necessary library

from huggingface_hub import login

#Data processing

import os

from transformers import GPT2Tokenizer

from docx import Document

from transformers import GPT2Tokenizer, OPTForCausalLM,Trainer, TrainingArguments, TextDataset, DataCollatorForLanguageModeling

import torch

from pyngrok import conf, ngrok

import subprocess

import time

