<b> 1. Compound–protein interaction prediction </b>: this is a binary classification task, which aims to predict if there is an interaction between the compound and the protein.

```
# Run at the commandline
python main.py -task interaction -dataset human
```

<b> 2. Compound–protein binding affinity prediction </b>: this is a regression task, which aims to predict a continuous value named binding affinity that reflects how tightly the compound binds to a particular target protein.

```
# Run at the commandline
python main.py -task affinity -dataset Kd
```

<b> 3. Specify hyperparameters </b>: there are many hyperparameters of the model (i.g. learning rate, batch size, epochs, step size, weight decay, hidden size, window size, layer size). For more information, please see the source code of main.py.

```
# Run at the commandline
python main.py -task affinity -dataset Kd -lr 0.001 -batch_size 64 -num_epochs 15
```
