# Developing a Pytorch CPP/CUDA Extension with a Makefile

[Pytorch cpp extensions](https://pytorch.org/tutorials/advanced/cpp_extension.html) provides a good way to augment pytorch with custom functions. The cpp-extension uses the setuptool to compile files. However, as it is mainly used for deployment rather than debugging and development, using the setuptool for development can be slow and cumbersome.

In this repository, I provide an alternative way to compile and debug your custom extension with a makefile.
The associated tutorial can be found at the [blog post](https://chrischoy.github.io/research/pytorch-extension-with-makefile).

## Installation

You must have `torch` installed in your current (virtual environment) python.

```
pip install -r requirements.txt
git clone https://github.com/chrischoy/MakePytorchPlusPlus
cd MakePytorchPlusPlus
make
```

For parallel compilation, use `make -j4` or any number of CPUs that you want to use.

## Running the example

```
python example.py
```
