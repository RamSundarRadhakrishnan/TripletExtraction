Triplet Extraction Notebook

A hands-on Jupyter notebook for extracting subject–predicate–object triplets from sentences using large language models (LLMs).

Filename: FinalTripletGenerator.ipynb

This single notebook contains all code to:

Load your sentences (from a CSV, text file, or inline list).
Configure and call the LLM - Gemma3 4B - through HuggingFace, and quantize the model to 4bit using Bitsandbytes.
Export extracted tripletsto CSV or JSON.

Dependencies:
Transformers
PyTorch
TQDM
Huggingface Hub

Requirements:
Python 3.8+
Jupyter Notebooks
An NVIDIA GPU is recommended - preferably one with support for bfloat16 (ie, Ada Lovelace and newer) for optimal performance.

Contributing and Feedback:
Please suggest improvements to the prompting, or the workflow!
You can contact me through ramsundar289@gmail.com

Notes:
Gemma3 4B can run on GPUs like the GTX 1050 4GB, but throughput is very low.
This notebook was tested on:
Pop!_OS + GTX 1050 -- batch size 8
Windows 11 + RTX 3050Ti -- batch size 8
H100 server environments -- batch size 256
Performance scaled well, and for best results the batch_size can be adjusted.
