# Image Captioning on Flickr8k

This repository contains a comparative study of three image captioning models evaluated on the Flickr8k dataset.  
Each model is implemented in an independent Jupyter notebook.

## Contents

- `ResNet50+LSTM_Flickr8k.ipynb`  
  CNN-based image captioning model with an LSTM decoder.

- `ResNet50+Transformer_Flickr8k.ipynb`  
  CNN-based image captioning model with a Transformer decoder.

- `BLIP2_LoRA_Flickr8k.ipynb`  
  Pretrained vision–language model (BLIP-2) adapted to image captioning using Low-Rank Adaptation (LoRA).

Each notebook is self-contained and can be executed independently.

---

## Dataset

All experiments are conducted on the **Flickr8k** dataset.

Please manually download the dataset from Kaggle:

👉 https://www.kaggle.com/datasets/adityajn105/flickr8k

After downloading, extract the dataset to a local directory or Google Drive.

### Important Note on Paths

The dataset paths in the notebooks are configured according to the original author's directory structure.  
To reproduce the experiments, you **must manually update all dataset-related paths** in each notebook to match your own setup.

This typically includes:
- Image directory paths
- Caption file path
- Train / validation / test split files

---

## Running the Code

To reproduce the results:

1. Open the notebooks (in any order, if desired):
   - `ResNet50+LSTM_Flickr8k.ipynb`
   - `ResNet50+Transformer_Flickr8k.ipynb`
   - `BLIP2_LoRA_Flickr8k.ipynb`
2. Modify the dataset paths according to your local or Colab environment.
3. Run all cells sequentially within each notebook.

No additional scripts are required.

---

## Environment

The notebooks were developed and tested using:

- **Google Colab**
- **NVIDIA A100 GPU**
- Python environment provided by Colab

For best reproducibility, running the notebooks on **Google Colab with GPU enabled** is recommended.  
The BLIP-2 + LoRA notebook requires GPU support and is the most computationally intensive.

---

## Notes

- Minor variations in runtime or numerical results may occur due to differences in hardware or environment.
- This repository is intended for educational and research purposes.

