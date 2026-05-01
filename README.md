# Legal SPO Extraction: OpenIE + GPT Intersection

Extracts legal obligation triples from CUAD contracts.

## Pipeline
CUAD contracts → OpenIE extraction → GPT validation → clause_predicate_dict

## Results
- 180 triples across 33 clause types
- 50 contracts processed
- OpenIE + GPT intersection for high precision

## Setup

### 1. Install dependencies
pip install spacy openai tqdm
python -m spacy download en_core_web_trf

### 2. Get the data files (not included — too large)
- CUAD dataset: https://www.atticusprojectai.org/cuad
  → download CUADv1.json → place in project root

- GPT triples: run gpt_extractor.ipynb first
  → generates gpt_triples_checkpoint.json

### 3. Run
Open maybe.ipynb and run all cells
Open and run pred.ipynb
