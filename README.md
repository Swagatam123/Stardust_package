# Stardust
Python package for cell-gene coembedding and analysis pipeline for single cell transcriptomics data


## Environment reqirements

Pyhton 3.7 or above with setuptools instaled.

## Installation Guide

Download the package directly from github. For linux users
```bash
git clone https://github.com/Swagatam123/Stardust.git
```
Download the binary openOrd.jar from the release tag v1.0 and place it under Stardust_package/stardust/run_stardust/
Change the directoery to the package directory
```bash
cd Stardust_package/
```
Use the package manager [pip](https://pip.pypa.io/en/stable/) to install package.

```bash
pip install .
```

## Dataset support fomrat

The package supports 10x genomics data with .10x file format and csv file with the filename expression.csv
The expression data should contain the cells rowwise and genes columnwise.

## Usage

```python
import stardust

stardust.run_stardust.run() #generated the coembedding plots under Stardust_resuts/visualization_output/4_pass.
stardust.analysis.silhouette() # optional for analysis purpose
stardust.analysis.heatmap()   # optional for analysis purpose
stardust.analysis.alluvial()  # optional for analysis purpose
```
## Output Directory structure
The embedding plots at its related data will be available in Stardust_results/visualization_output/4_pass

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

