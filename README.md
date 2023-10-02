# AI-Generated-Text-Detector

## For tackling the following problem of detecting AI generated text, I went through two major approaches:
## Benford's Law (Benford's_law.ipynb): 
It is the classic way of finding articial or tampered data in statistics. I tried using it for the task of detecting AI generated text by encoding text using tiktoken thus converting text to a large range of numbers. The results here were fairly mixed and didn't seem to conclude much

## Transformer Based Sequence Classification (Blog_Classification.ipynb and Blog_Classification_Inference.ipynb):
Here I used the roberta base sequence classifier and finetuned it on a dataset of 10000 AI generated and human written text. This model gave some more promising results and hence it was later converted to an onnx file and infered in a flask server for final application deployment.
