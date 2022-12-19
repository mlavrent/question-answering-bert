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

## Saved model

The model takes about 8 minutes per epoch to train. Since I have it training for 4 epochs, that's 30-40 minutes of training time. If you're just interested in running the model on some questions and documents, you can find the fine-tuned model [here](https://drive.google.com/file/d/1-7mIJ51anurqhHbGEJVw-QpUKP3lHfls/view?usp=sharing) (warning - 253 MB). To use it, make sure you put it in your repository as specified in the "How to run" section.

## Results

The model achieves the following results once fine-tuned:
```
precision: 0.64
recall:    0.69
f1-score:  0.61
```
