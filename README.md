# Medical Symptom Analysis with NLP

## Introduction
This repository contains code for leveraging Natural Language Processing (NLP) techniques to analyze medical symptoms. The program compares the performance of two models: a Named Entity Recognition (NER) model and the Viterbi algorithm as a baseline model for comparison.

## Project Structure
- `requirements.txt`: List of dependencies required to run the program.
- `label_list.txt`" List of labels found in the dataset.
- `inference.ipynb`: Script containing code for inferencing using the NER model.
- `ner_model.ipynb`: Script containing code for the NER model architecture and training.
- `viterbi_algorithm.ipynb`: Script containing code for the Viterbi algorithm implementation.

## Installation
1. ### Clone this repository: 

```
git clone https://github.com/karinnesagir/Symptom-Analysis
```

2. ### Install dependencies:

```
pip install -r requirements.txt

```

3. ### Download the Pre-trained NER Model

   #### Files Included
   The folder `ner_model` contains two essential files:
   - `config.json`: Configuration settings for the BERT model.
   - `model.safetensors`: Serialized model weights in SafeTensors format.
  
   #### Steps to Download
   1. Visit the Google Drive link: [Download NER Model](https://drive.google.com/drive/folders/1o-jS-64JpAx0QALsyeoWa8H_T5SP2MxL?usp=sharing)
   2. Download the entire `ner_model` folder and place it in the root directory of this repo.
   

## Usage

### Named Entity Recognition Using BERT

#### Training
To train the model, follow these steps:
1. Open and run the `NER.ipynb` notebook.

   Configuration details:
   - **Epochs**: 100
   - **Batch Size**: 32
   - **Learning Rate**: 0.00002 (2e-5)
   - **Evaluation Strategy**: Per epoch
   - **Weight Decay**: 0.01
   - **Tokenizer**: `bert-base-uncased`
   - **Data Collator**: Use `DataCollatorForTokenClassification` from the transformers library.

#### Inferencing
For model inference:
1. Ensure the `ner_model` folder is downloaded to the root directory of this repository.
2. Open and run the `inference.ipynb` notebook.

### Named Entity Recognition Using Viterbi Algorithm
To run the model, open and run the `viterbi.ipynb` notebook.


## Results

### Performance Metrics

The evaluation of both models is performed on test data that was previously unseen by the models, ensuring the reliability of the metrics.

#### NER Model
The Named Entity Recognition (NER) model provides a comprehensive set of performance metrics:
- **Accuracy**: 88.66%
- **Precision**: 74.92%
- **Recall**: 78.24%
- **F1 Score**: 76.54%

These metrics help in understanding the model's effectiveness in identifying named entities across various classes.

#### Viterbi Algorithm
The Viterbi algorithm, used for sequence prediction, reports its effectiveness as follows:
- **Accuracy**: 78.45%

This metric reflects the algorithm's accuracy in predicting the most likely sequence of states.

### Conclusion

The NER model demonstrates a significant improvement over the Viterbi algorithm, highlighting its robustness in Named Entity Recognition tasks. With an accuracy of 88.66%, the NER model proves particularly effective in complex scenarios, such as analyzing medical texts, where precision and context are critical. This enhancement indicates the NER model's superior ability to handle nuanced language and structure inherent in specialized domains.

## Contributing
Contributions are welcome! If you find any issues or have suggestions for improvement, please open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

