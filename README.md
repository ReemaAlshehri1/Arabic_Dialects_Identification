# Arabic_Dialects_Identification

- In this project i bfine-tunes AraBERT model using LoRA to identify which arabic dialect the giving sentence is.
- The model can predict weather the sentence  belongs to these 6 dialects:
 - Eygypt
 - Gulf
 - Magreb
 - Levant
 - Msa
 - Sudan

## Features
- Fine-tuning AraBERT  model
- Using LoRA technique
- Using 3 datasets 
- Built with Gradio interface

  
## Dataset
For this project i used 3 Datasets from Kaggle to resolve classes imbalance
- [Arabic_dialect](https://www.kaggle.com/datasets/waelshaher/arabic-dialect)
- [ArSarcasm](https://www.kaggle.com/datasets/hosammohammed/arabic-dataset)
- [BERT_Arabic_Dialect](https://www.kaggle.com/datasets/hanahelaly/bert-arabic-dialect)

**Preprocessing steps:**
- Applied a function for text cleaning .
- Used AraBERT preprocessing for normalization.


## How to run
1. clone the repository:
   ```bash
   git clone https://github.com/ReemaAlshehri1/arabic-dialect-identification.git
   cd arabic-dialect-identification
2. Install required dependencies:
   ```bash
   pip install -r requirements.txt
3.Download the datasets from the Kaggle links above
4. Open and run `Arabic_dialects_detection.ipynb` in Google Colab or Jupyter Notebook:
 - This will preprocess the dataset, fine-tune the AraBERT model with LoRA, and save the model weights.
5. Run the app.py:
   ```bash
   python app.py.py
 - This will start a Gradio interface for live predictions.
   
## Results
- The accuracy of the model showed 81%
  
## Github structure
- `Arabic_dialects_detection.ipynb` – Main notebook for training and evaluation
- `app.py` – Gradio interface for live predictions
- `requirements.txt` – Required dependencies
- `arabert-dialect-lora/` – Fine-tuned model weights (or Hugging Face model link)
- `README.md` – Project documentation

## Licesns

