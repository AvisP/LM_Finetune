# LM_Finetune
This repo contains few notebooks on fine tuning of Language Models. They are based on fine tuning examples that were publicly available. Objective was to familiarize with training process and overcome the technical challenges associated with training on limited GPU resources and package versioning issues. Details of each notebook are provided below

* **transformers_causallanguagemodelling.ipynb** : This contains a fine tuning method of the ***wikitext*** dataset on the **distilgpt*** model and inference once the training has finished using the **Trainer** API
* **gpt2-shakespeare-trainargs.ipynb** : It contains fine tuning of ***GPT 2*** model on ***shakespeare*** writings using the ***Trainer*** API. ( Has a bit of issue with generating train and test set that needs to be completed.)
* **transformer-clm-distilgpt-eli5.ipynb** : It contains fine tuning of ***GPT 2*** model on ***eli5*** dataset using the Trainer API and inference as well
* **gemma-7b-it-fine-tune-roleplay.ipynb** : It contains fine tuning of Google's **Gemma 7B** model after loading it up in 4 bit format, LORA adapters inserted and then trained using the Trainer API. Dataset used is the open source ***hieunguyenminh/roleplay***.
* **gemma-7b-it-inference-roleplay.ipynb** : This script show how to do inferencing, once the Lora model is trained in the training notebook. The trained LORA adapters are merged with the the base ***Gemma 7B model*** before inferencing
* **mistral-7b-instruct-fine-tuning-qlora.ipynb** : This notebook shows how to do QLORA finetuning using ***Mistral-7B-instruct*** model on the ***HuggingFaceH4/ultrachat_200k*** open source dataset
* **mistral-7b-instruct-inference-qlora.ipynb** : This script shows how to do QLORA inferencing using ***Mistral-7B-instruct***, once the Lora model has been trained by merging with the base model
* **llama-3-finetune-qlora.ipynb** : This notebook shows how to perform finetuning on Meta's ***LLAMA-3-8B-Instruct*** model after loading it up in 4 bit format. LORA adapters inserted with appropriate ranks and then trained using the Trainer API. Dataset used is ***HuggingFaceH4/ultrachat_200k***
* **llama3-qlora-inference.ipynb** : This notebook shows how to do QLORA inferencing using ***LLAMA-3-8B-Instruct*** model after it has been finetuned after merging with the base model.
* **Beam_Llama3-8B-finetune_task.py** : This script shows how to start a fine tuning task on beam.cloud, a serverless cloud infrastructure.
