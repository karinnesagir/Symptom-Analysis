# Medical Symptom Analysis with NLP

## Introduction
This repository contains code for leveraging Natural Language Processing (NLP) techniques to analyze medical symptoms. The program compares the performance of two models: a Named Entity Recognition (NER) model and the Viterbi algorithm as a baseline model for comparison.

## Project Structure
- `requirements.txt`: List of dependencies required to run the program.
- `main.py`: Main script to execute the program and compare the NER model and Viterbi algorithm.
- `ner_model.py`: Script containing code for the NER model architecture and training.
- `viterbi_algorithm.py`: Script containing code for the Viterbi algorithm implementation.

## Installation
1. Clone this repository: 

```
git clone https://github.com/karinnesagir/Symptom-Analysis
```

2. Install dependencies:

```
pip install -r requirements.txt

```

## Usage
1. Ensure you have the necessary datasets in the `data/` directory.
2. Run the main script to compare the NER model and Viterbi algorithm:

```
python main.py
```

# Results
The program will output the performance metrics of both the NER model and Viterbi algorithm, including accuracy, precision, recall, and F1 score.

## Contributing
Contributions are welcome! If you find any issues or have suggestions for improvement, please open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

