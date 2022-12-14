# run_matlab
**Command Line MATLAB Function Caller with Automatic MATLAB Compiler Runtime (MCR) Installation**

[![PyPI version](https://badge.fury.io/py/run_matlab.svg)](https://badge.fury.io/py/run_matlab)
[![DOI](https://zenodo.org/badge/522426883.svg)](https://zenodo.org/badge/latestdoi/522426883)
<br/>

# Installation
```shell
pip3 install run_matlab
```

# Usage
```shell
run_matlab <command> [options]
Commands:
    install            Installation of the MATLAB compiler runtime (MCR)
    run                Running the MATLAB function after installation
Run run_matlab <command> -h for help on a specific command.

run_matlab: Command Line MATLAB Function Caller with Automatic MATLAB Compiler
Runtime (MCR) Installation

positional arguments:
  command     Subcommand to run

optional arguments:
  -h, --help  show this help message and exit
  --version   show program's version number and exit
```

## Initialization of MATLAB Compiler Runtime (MCR)
```shell
run_matlab install [-h] [-d INSTALLATION_DIR] [-v MATLAB_VERSION]
                          [-r RUNTIME_VERSION]

Installation of the MATLAB compiler runtime (MCR)

optional arguments:
  -h, --help           show this help message and exit
  -d INSTALLATION_DIR  Directory wherein the MATLAB compiler runtime (MCR)
                       will be installed. (default: $HOME/run_matlab)
  -v MATLAB_VERSION    MATLAB version. (default: R2013b)
  -r RUNTIME_VERSION   MATLAB Compiler Runtime version. (default: 8.2)
```

| MATLAB_VERSION  | RUNTIME_VERSION |
| ------------- | ------------- |
| R2013b | 8.2 |
| R2014a | 8.3 |
| R2014b | 8.4 |
| R2015a | 8.5 |
| R2015b | 9.0 |
| R2016b | 9.1 |
| R2017a | 9.2 |
| R2017b | 9.3 |
| R2018a | 9.4 |
| R2018b | 9.5 |
| R2019a | 9.6 |
| R2019b | 9.7 |
| R2020a | 9.8 |
| R2020b | 9.9 |

## Execution of MATLAB Functions
```shell
run_matlab run [-h] [-d INSTALLATION_DIR] [-v MATLAB_VERSION]
                      [-r RUNTIME_VERSION]
                      function_dir function_name
                      [function_args [function_args ...]]

Running the MATLAB function after installation

positional arguments:
  function_dir         Directory wherein the standalone MATLAB function is
                       located.
  function_name        Name of the standalone MATLAB function.
  function_args        Arguments for the standalone MATLAB function. (default:
                       None)

optional arguments:
  -h, --help           show this help message and exit
  -d INSTALLATION_DIR  Directory wherein the MATLAB compiler runtime (MCR) was
                       installed. (default: $HOME/run_matlab)
  -v MATLAB_VERSION    MATLAB version. (default: R2013b)
  -r RUNTIME_VERSION   MATLAB Compiler Runtime version. (default: 8.2)
```
