# nmt-english-to-tamil
Fine-tuning MarianMT neural machine translation model for English to Tamil using LoRA and the Samanantar dataset.
## What is this project about?
This project fine-tunes a neural machine translation (NMT) model called MarianMT to translate sentences from English to Tamil.

MarianMT is a pre-trained language model specialized in translation tasks.

Instead of training from scratch, this project improves MarianMT using LoRA adapters, which make fine-tuning faster and more efficient by training only a small part of the model.

The model is trained with a large dataset called Samanantar, which has pairs of English and Tamil sentences for learning translation.
## Key concepts explained simply
### 1. Neural Machine Translation (NMT)
It is an AI technique that converts text from one language to another using deep learning models.

Models like MarianMT can learn how to translate by studying large examples (data sets).
### 2. MarianMT
It is an open-source transformer-based model made specifically for machine translation.

You start with MarianMT already trained on many languages, then refine it for English-to-Tamil with your data.
### 3. LoRA (Low-Rank Adaptation)
LoRA is a method that helps you fine-tune big models with fewer resources.

Instead of updating all model weights, LoRA updates a smaller set of parameters, making training easier and faster.

### 4. Samanantar Dataset
This is a big parallel corpus (dataset) containing paired English and Tamil sentences.

The model learns to translate by seeing many correct sentence pairs.
## Description
This project performs neural machine translation from English to Tamil by fine-tuning the MarianMT model using LoRA adapters. Training was conducted on the Samanantar dataset, and the included code demonstrates the complete training process.
## Installation
1. Clone this repository:
   git clone https://github.com/Narmadas-31/nmt-english-to-tamil.git
   
 ```python
   cd nmt-english-to-tamil
 ```
3. Install dependencies:
   
 ```python
   pip install -r requirements.txt
  ```
## Usage
- To train the model or view training progress, open the included Jupyter notebook:
  jupyter notebook notebook21d9e9b179-2.ipynb
- Example: Run all notebook cells to fine-tune the model, validate, and see results.
- To visualize logs, in a notebook cell:
 ```python
%load_ext tensorboard
%tensorboard --logdir ./logs
```
- Training/validation loss and performance metrics are displayed in the notebook.

## Features
- Fine-tunes MarianMT for English-to-Tamil machine translation
- Implements parameter-efficient LoRA adapters
- Uses Samanantar dataset for robust, real-world performance
- Includes loss table, TensorBoard logging, and inference examples

## Dataset
Trained on the Samanantar parallel corpus for English–Tamil.

## Contributing
Pull requests are welcome!  
For major changes, please open an issue to discuss what you’d like to add or change.

## License
This project is licensed under the MIT License.


 


