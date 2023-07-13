# ICCS Summer School '23: Introduction to Hugging Face -- Model code
This repository stores a simple Python script which trains a Pytorch model
(adapted from an example in
https://github.com/pytorch/examples/tree/7f7c222b355abd19ba03a7d4ba90f1092973cdbc).

## Using
### Dependencies
Python 3.

Requires Python libraries `torch` and `torchvision`. With `pip`:

    pip install -r requirements.txt

### Development environment
#### virtualenv
You may using `virtualenv` to create a self-contained Python environment for
this project. In your shell, in the root of the repository, with `virtualenv`
and `pip` installed, run:

    virtualenv venv
    source venv/bin/activate
    pip install -r requirements.txt

The `source` command sets up your shell to use the self-contained environment
until you close it. Every time you want to use it, run `source
venv/bin/activate` in the directory you created the virtualenv in.

#### Nix
A Nix flake including a devshell is provided for Nix users. `nix develop` will
set up requirements to then follow the `virtualenv` instructions above. (Your
Nix version needs to support flakes.)

### Training and saving model
    python main.py --save-model

(The default epochs has been retuned from 14 to 3 for faster execution by
default. Change this by adding an `--epochs x` option.)
