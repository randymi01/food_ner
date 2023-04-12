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

## License

[MIT](https://choosealicense.com/licenses/mit/)
