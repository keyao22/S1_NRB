# S1-NRB prototype processor

https://sentinel.esa.int/web/sentinel/sentinel-1-ard-normalised-radar-backscatter-nrb-product

## Installation

- Install and then activate conda environment: 
```bash
conda env create --file environment.yaml
conda activate nrb_env
```

- Install this package into the environment:
```bash
pip install .
```

## Usage

- Create a config file (see `config.ini` for an example) and store it in your project directory
- Print a help message using:
```bash
s1_nrb --help
```

- Start the processor using parameters defined in a config file:
```bash
s1_nrb -c /path/to/your/config.ini
```

A description of individual steps can be found [here](https://github.com/SAR-ARD/S1_NRB/blob/main/docs/S1_NRB.rst).

## Update
The latest states of `pyroSAR` and `spatialist`, which are developed alongside `S1_NRB`, can be updated like this:
````shell
pip install git+https://github.com/johntruckenbrodt/spatialist.git --upgrade --no-deps --force-reinstall
````
