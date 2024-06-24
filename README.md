# Wisconsin Breast Cancer Dataset Analysis - A Guideline for Developing Scripts within Federated Learning

This repository provides comprehensive guidelines on how scripts are developed for the Federated Learning for Everyone (FL4E) framework using the [Wisconsin Breast Cancer Dataset](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+(Diagnostic)). 

## Structure of the Repository

The repository is divided into several directories, each serving a unique purpose:

1. **data Folder**: This folder contains slices of the original Wisconsin Breast Cancer dataset, labeled as "_1" and "_2". 

2. **centralised Folder**: Here you'll find an empty data dictionary CSV file corresponding to the Wisconsin Breast Cancer dataset. This file serves as the first step of data sharing within the Data Center of FL4E. Moreover, this folder contains a sample data cleaning script and two sliced CSV files from the main dataset, as if we have two clients wanting to share data centrally.

3. **src Folder**: This folder houses necessary scripts, namely `client.py`, `server.py` and `utils.py`, which should be uploaded in the Study Center. Clients must download and execute `client.py` and `utils.py` on the FL4E client docker component. `server.py` and `utils.py` should be executed by study lead. Study lead must upload and execute these scripts on their desired machine, however IP and Port address should be communicated to the participants. 

At the end of training, the model and weights can be downloaded and uploaded back to the model center of FL4E.

## Detailed explanation

Required software to run the python scripts in Python, required packages can be found in requirements.txt and can be installed as `pip install -r requirements.txt` or `pytho3 -m pip install -r requirements.txt`

The various markdown files provide a layman explanation of each part of the code that walks an interested layman party through the code step-by-step. 

- [server](server.md)
- [client](client.md)
- [utils](utils.md)