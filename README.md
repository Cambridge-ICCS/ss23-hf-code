# ICCS Summer School '23: Introduction Hugging Face -- Model code
This repository stores a simple Python script which trains a Pytorch model
(adapted from an example in
https://github.com/pytorch/examples/tree/7f7c222b355abd19ba03a7d4ba90f1092973cdbc).

## Using
### Dependencies
Python 3.

Requires Python libraries `torch` and `torchvision`. With `pip`:

    pip install -r requirements.txt

### Training and saving model
`python main.py --save-model`

(The default epochs has been retuned from 14 to 3 for faster execution by
default. Change this by adding an `--epochs x` option.)
