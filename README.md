# Project Introduction
Lightweight fine-tuning is one of the most important techniques for adapting base models, as it allows you to modify these models to suit your needs without requiring substantial computational resources.

This project is from the course Generative AI from UDACITY In this project we apply parameter-efficient fine-tuning using Hugging Face’s `peft` library.
PEFT technique: LoRA, as it enables efficient fine-tuning for LLMs. 
Model: DistilBERT, which allows for rapid fine-tuning with minimal hardware resources. 
Evaluation approach: precision and loss metrics. 
Fine-tuning dataset: SMS Spam, as it aligns with the project’s requirements of using small, easy-to-handle datasets.

# Run in your own computer

To run in my own laptop was a little tricky.
To create the enviroment in your computer with CUDA I use this command:

pip install torch torchvision torchaudio transformers --index-url https://download.pytorch.org/whl/nightly/cu130

Also you need:
pip install pandas, matplotlib

In `datasets` 3.0.1, an iterable stream was converted to a `DataFrame` without attempting to cast complex columns (such as lists of structs). However, as of `datasets` 3.6.0, a change was introduced in how features and PyArrow are handled. So you can use:
pip install datasets==3.0.1

pip install transformers[torch]
pip install peft
pip install scikit-learn

conda install jupyter notebook
