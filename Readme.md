# OpenPIV 2.0 plan

Think about making a website and best practice tutorial that explains to users how to navigate the complex OpenPIV world. How do you choose between C++, Python, and Matlab, and what are the features and pros/cons you get if you choose something? In the Python world, there are already plenty of fast solutions: PyFFTW, Numba, single-precision, etc., but if the speed is the main issue, then the user could jump to C++, yet with the same set of parameters. It's essential to have the same set of inputs basically and the same set of outputs (one single data type for the PIV files) and translators or transparent layers that allow as little effort as possible to move and upgrade the analysis from the simplest one `run_openpiv(frame_1, frame_2)` that could become `run_openpiv(frame_1, frame_2, method='extended')` or `run_openpiv(frame_1, frame_2, method='cuda', settings = default_settings)` and `run_openpiv(frame_1, frame_2, method='c++', settings=default_settings).` 

## Decisions:
1. we use Python as a glue
2. we use Jupyter Notebooks as a first-order GUI; we keep Python scripts in the bash/command prompt for the batch runs. We use Jupyter notebooks for the first visualization steps and tutorials
3. we avoid complex installations unless the user understands what is required and pre-installs successfully
4. 


## simple first step:
1. create a Jupyter notebook that runs openpiv-python, openpiv-python-cpu, and openpiv-python-gpu using the same set of parameters
2. think about Python packaging and management


## OpenPIV tree that we want to unify (not in a specific order, but we shall start simple with Python):
1. https://github.com/OpenPIV/openpiv-python
2. https://github.com/ali-sh-96/openpiv-python-cpu
3. https://github.com/ali-sh-96/openpiv-python-gpu
4. https://github.com/OpenPIV/openpiv-python-gpu
5. https://github.com/ErichZimmer/OpenPIV-Python-cxx
6. https://github.com/OpenPIV/openpiv-c--qt
7. 

## Co-authors

1. @ali-sh-96
2. @alexlib
3. Please join us
