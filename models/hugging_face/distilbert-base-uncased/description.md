The DistilBERT base model (uncased) is a distilled version of the BERT base model that is smaller and faster than BERT. It was introduced in a specific paper and the code for creating the model can be found on a specific webpage. The model is uncased so it doesn't differentiate between lower and upper case letters in the English language. DistilBERT is considered a transformers model that was pretrained on the same corpus in a self-supervised fashion using the BERT base model as a teacher. The model was pretrained using the distillation loss, masked language modeling, and cosine embedding loss objectives. The intended use of the model is to be fine-tuned on downstream tasks like sequence classification, token classification, and question answering, but not text generation.

> The above summary was generated using ChatGPT. Review the [original model card](https://huggingface.co/distilbert-base-uncased) to understand the data used to train the model, evaluation metrics, license, intended uses, limitations and bias before using the model.

### Inference samples

Inference type|Python sample (Notebook)|CLI with YAML
|--|--|--|
Real time|[sdk-example.ipynb](https://aka.ms/azureml-infer-sdk)|[cli-example.sh](https://aka.ms/azureml-infer-cli)
Batch | todo


### Finetuning samples

Task|Use case|Dataset|Python sample (Notebook)|CLI with YAML
|---|--|--|--|--|
Text Classification|Emotion Detection|[Emotion](https://huggingface.co/datasets/dair-ai/emotion)|[emotion-detection.ipynb](https://aka.ms/azureml-ft-sdk-emotion-detection)|[emotion-detection.sh](https://aka.ms/azureml-ft-cli-emotion-detection)
Token Classification|Token Classification|[Conll2003](https://huggingface.co/datasets/conll2003)|[token-classification.ipynb](https://aka.ms/azureml-ft-sdk-token-classification)|[token-classification.sh](https://aka.ms/azureml-ft-cli-token-classification)
Question Answering|Extractive Q&A|[SQUAD (Wikipedia)](https://huggingface.co/datasets/squad)|[extractive-qa.ipynb](https://aka.ms/azureml-ft-sdk-extractive-qa)|[extractive-qa.sh](https://aka.ms/azureml-ft-cli-extractive-qa)


### Model Evaluation

|Task|Use case|Dataset|Python sample (Notebook)|
|---|--|--|--|
|Fill Mask||[imdb](https://huggingface.co/datasets/imdb)|[evaluate-model-fill-mask.ipynb](https://aka.ms/azureml-eval-sdk-fill-mask/)|