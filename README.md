# conx2
conx is a small neural network library at https://github.com/ArtificialIntelligenceToolkit/conx that stopped working when keras got absorbed into tensorflow. 

So I cloned it and fixed it. All you need to do is to `pip install tensorflow` after you pip install conx2 from github like so:
```
python -m pip install git+https://github.com/dinorows/conx2
```

FYI, I create a new python 3.7-based environment for this (just in case you have issues with higher versions of python).

You probably also want to:
```
pip install pyqt5
```

And then, in order to plot straight to your notebook while your network is training, add a cell with this code in your notebook:
```
import matplotlib
import matplotlib.pyplot as plt
matplotlib.use('Qt5Agg')
%matplotlib inline
```

Enjoy!


