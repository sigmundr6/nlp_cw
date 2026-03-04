# NLP Coursework

This repository contains the code and dataset to reproduce the results for the NLP coursework.

## Dataset Location

The dataset files are located in the `BestModel/` directory:
- `BestModel/dontpatronizeme_pcl.tsv`
- `BestModel/task4_test.tsv`
- `BestModel/train_semeval_parids-labels.csv`
- `BestModel/dev_semeval_parids-labels.csv`

The data files are structured as TSV and CSV formats and contain the annotations and text inputs necessary for training and evaluation.

## How to Reproduce

To reproduce the results, you need to run the Jupyter Notebook in the `BestModel` directory:

```bash
cd BestModel
jupyter notebook train_lora_ensemble.ipynb
```

### Steps inside the notebook:
1. Ensure your Python environment has the required dependencies installed. A `requirements.txt` file has been provided in the root directory. You can install all necessary dependencies by running:
   ```bash
   pip install -r requirements.txt
   ```
2. The notebook expects the underlying dataset files to reside in the same folder (`BestModel/`).
3. Run all cells in `train_lora_ensemble.ipynb` in order.
4. The notebook will process the data, perform model training or inference, and output the resulting predictions/metrics.

## File Hierarchy

```
nlp_cw/
├── BestModel/
│   ├── dev_semeval_parids-labels.csv
│   ├── dontpatronizeme_pcl.tsv
│   ├── ensemble_loras/
│   ├── task4_test.tsv
│   ├── train_lora_ensemble.ipynb
│   └── train_semeval_parids-labels.csv
├── dev.txt
└── test.txt
```
