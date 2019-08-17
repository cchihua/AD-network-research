
# AD Network Analysis Notebook

The AD Network Analysis Notebook is a introductory Jupyter Notebook that demonstrates the use of the modules in the UCSD CCBB's [network-bio-toolkit](https://github.com/ucsd-ccbb/network_bio_toolkit) to analyze AD and AD GWAS genes.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development purposes.

### Prerequisites

* UCSD CCBB's [network-bio-toolkit](https://github.com/ucsd-ccbb/network_bio_toolkit): Follow the documentation for installation procedure.
##### Note: Must use ndex2 version 1.2.0.56 (`pip install ndex2==1.2.0.56`), and networkx version 1.11 (`pip install networkx==1.11`)
* [Jupyter Notebook](https://jupyter.org/) (Anaconda install recommended.)
* Python

### Required Files

* **AD Genes**: [Agora Target List](https://agora.ampadportal.org/genes/)
* **AD GWAS Genes**: [AD-by-proxy FUMA GWAS List (Table S13)](https://www.nature.com/articles/s41588-018-0311-9)
* **Heat DG Universe**: provided .gpickle file (located in the `data/` folder)
##### Copies of all files are provided in the `data/` folder.

### Installing

After setting up the prerequisites, clone the repository using an OS terminal with Git installed, or download the repository code.

```
git clone https://github.com/nhtsai/AD-network-research.git
```

And locate the `ADNetworkNotebook/` folder.
```
cd ADNetworkNotebook/
```

Use Jupyter to open the `ADNetworkAnalysis.ipynb` notebook file and run the cells.

**Note:** Lines of code with `os.path.join()`,  are meant to locate the paths to the required files listed above and your local installation of the [network-bio-toolkit](https://github.com/ucsd-ccbb/network_bio_toolkit). This is optional but allows for greater compatibility, as file-paths between Windows and Mac can be different in some scenarios. To use this function, separate directory and file names with commas.

For example, if the `network-bio-toolkit` was downloaded in `./Downloads/`, the relative path to it would be `./Downloads/network-bio-toolkit`. Using `os.path.join()`, this would look like `os.path.join('Downloads', 'network-bio-toolkit')`.

Using a string of the absolute/relative path (e.g. `/Users/username/Downloads/network-bio-toolkit`) can work as the path variable and may be simpler.

## Authors

* **Nathan Tsai** - [nhtsai](https://github.com/nhtsai)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
