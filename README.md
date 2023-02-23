# conx2
conx is a small neural network library at https://github.com/ArtificialIntelligenceToolkit/conx that stopped working when keras got absorbed into tensorflow. 

So I cloned it and fixed it. But you will need a python 3.7 based distribution.

All you need to do is to create a new python 3.7-based environment called `conx2` (or anything else you wish), either through anaconda navigator or in an anaconda shell with `conda create -n conx2 python=3.7`. 

Then, open an anaconda shell and activate that environment with `conda activate conx2`, followed by pip-installing conx2 from github like so:
```
python -m pip install git+https://github.com/dinorows/conx2
```

Then, follow by installing tensorflow:
```
pip install tensorflow
```

You probably also want to:
```
pip install pyqt5
```

In order to plot conx loss and accuracy graphs straight to your notebook while your network is training, add a cell with this code in your jupyter notebook:
```
import matplotlib
import matplotlib.pyplot as plt
matplotlib.use('Qt5Agg')
%matplotlib inline
```

Make sure to run your notebook within your new environment by switching to your `conx2` kernel.

Other than that, your old conx-based python notebooks should not need to be modified at all. In other words, import `conx`, not `conx2:
```
import conx as cx
```

and keep on computing!
