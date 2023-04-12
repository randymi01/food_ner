# Food NER

Spacy Food Name Entity Recognition (NER) model trained on StanfordNLP CRF recipe dataset

## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install spacy version spacy==3.5.0 and then download the spacy en_core_web_sm model.

```bash
pip install spacy==3.5.0
python -m spacy download en_core_web_sm
```

## Usage

```python
import spacy

nlp = spacy.load("model")

# returns (spring mix, chicken breast, chili, hamburger meat)
nlp("I have spring mix, chicken breast, chili, and hamburger meat").ents

```

## Model Hyperparameters 
* Epochs: 10
* Batch Size: 4-32
* Optimizer: Adam
* lr = 5e-03
* drop_rate = 0.5

## Model Performance
![alt text](https://github.com/randymi01/food_ner/blob/main/training_loss.png?raw=true)
![alt text](https://github.com/randymi01/food_ner/blob/main/validation_loss.png?raw=true)

## License

[MIT](https://choosealicense.com/licenses/mit/)
