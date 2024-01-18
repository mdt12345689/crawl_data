# VietnameseTextToxicClassify
I train this model using PyTorch to detect toxic of a comment for Projectube

I use VNCoreNLP for preprocess the raw Vietnamese sentences data and PhoBERT to train model to classify text. I use these technology at https://github.com/VinAIResearch/PhoBERT.

## Use my code


###  Change directory to my folder and install VNCoreNLP:
```
cd VietnameseTextToxicClassify
pip3 install vncorenlp
mkdir -p vncorenlp/models/wordsegmenter
wget https://raw.githubusercontent.com/vncorenlp/VnCoreNLP/master/VnCoreNLP-1.1.1.jar
wget https://raw.githubusercontent.com/vncorenlp/VnCoreNLP/master/models/wordsegmenter/vi-vocab
wget https://raw.githubusercontent.com/vncorenlp/VnCoreNLP/master/models/wordsegmenter/wordsegmenter.rdr
mv VnCoreNLP-1.1.1.jar vncorenlp/ 
mv vi-vocab vncorenlp/models/wordsegmenter/
mv wordsegmenter.rdr vncorenlp/models/wordsegmenter/
```
###  Add more data in 2 json files

###  Run training file:
```
python3 training.py
```
---
### HOANG CAO BAO
