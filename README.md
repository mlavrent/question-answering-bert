# Question answering
Final project for cs1460 (Computational Linguistics)
- cs login: mlavrent
- paper: [A BERT Baseline for the Natural Questions](https://arxiv.org/pdf/1901.08634.pdf)

## How to run
The notebook relies on being in a Google Drive drive with the following hierarchy:
```
MyDrive
└- Colab Notebooks
   ├- qa-final-data/
   │  ├─ dev.json
   │  └- train.json
   ├- qa-model.model (optional, if loading from saved model)
   └- qa-final.ipnyb
```
In other words, just put this repository in `MyDrive/Colab Notebooks` and you should be all set.

If `qa-model.model` is present, the notebook will just load the saved fine-tuned model and avoid training again (this may help for running quickly). If it isn't present, it'll fine-tune the model again.


