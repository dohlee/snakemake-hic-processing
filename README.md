# snakemake-hic-processing

Hi-C processing pipeline in snakemake.

This pipeline takes cares of (optional) download of raw sequencing reads from sequencing read archives, alignment using `bwa`, `.pairs` or `.pairsam` file generation and pair filtering using `pairtools`, and finally contact matrix generation using `cooler`.

## Quickstart

1. Clone the repo.

```
$ git clone https://github.com/dohlee/snakemake-hic-processing.git
$ cd snakemake-hic-processing
```

2. Modify the configuration `config.yaml` and `manifest.csv` as you want.

3. Create conda environment for this pipeline and run it. Consider using `mamba` if downloading packages takes long time. 

```
$ conda env create -f environment.yaml
```

## See also

This pipeline is mostly similar to the official Hi-C Processing Pipeline in 4D nucleome project: https://data.4dnucleome.org/resources/data-analysis/hi_c-processing-pipeline. See also the official github repository https://github.com/4dn-dcic/docker-4dn-hic/tree/v43.
