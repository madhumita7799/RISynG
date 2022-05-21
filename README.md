# RISynG
Recursive Integration of Synergised Graph Representations of Multi-omics Data for Cancer Subtypes Identification


## Installation

### Clone the repository 
Download the package and change your working directory to `RISynG/`

### Install dependencies

```
$ pip3 install pipenv
$ pipenv install

```

### Activate the virtual environment

```
$ pipenv shell

```

## Usage
Add executable permission to the provided `run.sh` script.
```
$ chmod +x run.sh

```
There are five dataset in the `Datasets` folder- OV, STAD, CESC, LGG and BRCA. The algorithm can be executed for these dataset through the provided shell script `run.sh` as illustrated below.

```
$ ./run.sh dataset # replace 'dataset' with the name of the dataset

```
Execution can be done for multiple dataset just by cascading the names one after the other.

### MANUAL
```
usage: risyng [-h] [--fuse [FUSE]] [--dataset [DATASET]] [--modality [MODALITY]] [--bval [BVAL]] [--order [ORDER]] [--cluster [CLUSTER]]

optional arguments:
  -h, --help            show this help message and exit
  --fuse [FUSE], -f [FUSE]
                        Pass 'y' for fusion.
  --dataset [DATASET], -d [DATASET]
                        Which dataset?
  --modality [MODALITY], -m [MODALITY]
                        Which modality? (an integer)
  --bval [BVAL], -b [BVAL]
                        At what b? (a number, or 'N' for default)
  --order [ORDER], -o [ORDER]
                        In what oder?
  --cluster [CLUSTER], -k [CLUSTER]
                        Number of clusters
```

## OUTPUT
```
Gmat/~: Contains synery matrices
intWA/~: Contains intergrated matrices
labels/~: Contains class labels

```





