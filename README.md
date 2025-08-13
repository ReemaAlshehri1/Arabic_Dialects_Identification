# Arabic_Dialects_Identification

- In this project i fine-tuned AraBERT model using LoRA to identify which arabic dialect the giving sentence is.
- ![Interface Screenshot](images/gradio_interface.png)
- The model can predict wheather the sentence belongs to these 6 dialects:
 - Eygpt
 - Gulf
 - Maghreb
 - Levant
 - Msa
 - Sudan

## Features
- Fine-tuning AraBERT  model
- Using LoRA technique
- Using 3 datasets from Kaggle
- Gradio interface for live predictions

  
## Dataset
For this project i used 3 Datasets from Kaggle to resolve classes imbalance
- [ArSarcasm](https://www.kaggle.com/datasets/hosammohammed/arabic-dataset)
- [BERT_Arabic_Dialect](https://www.kaggle.com/datasets/hanahelaly/bert-arabic-dialect)
- [Arabic_dialect](https://www.kaggle.com/datasets/waelshaher/arabic-dialect)

**Preprocessing steps:**
- Applied a function for text cleaning.
- Used AraBERT preprocessing for normalization.


## How to run
1. clone the repository:
   ```bash
   git clone https://github.com/ReemaAlshehri1/arabic-dialect-identification.git
   cd arabic-dialect-identification
2. Install required dependencies:
   ```bash
   pip install -r requirements.txt
3. Download the datasets from the Kaggle links above.
   - If running in Google Colab, you can download them directly in the notebook by adding your own Kaggle API credentials and adjusting the dataset paths in the cells.  
   - If running locally, download the datasets manually and update the dataset paths in `Arabic_dialects_detection.ipynb` .
4. Open and run `Arabic_dialects_detection.ipynb` in Google Colab or Jupyter Notebook:
   - This will preprocess the dataset, fine-tune the AraBERT model with LoRA, and save the model weights.
5. Run the app.py:
   ```bash
   python app.py
 - This will start a Gradio interface for live predictions.
   
## Results
- The accuracy of the model showed 81%
  
## Github structure
- `Arabic_dialects_detection.ipynb` – Main notebook for training and evaluation
- `app.py` – Gradio interface for live predictions
- `requirements.txt` – Required dependencies
- `arabert-dialect-lora/` – Fine-tuned model weights 
- `README.md` – Project documentation

## License

