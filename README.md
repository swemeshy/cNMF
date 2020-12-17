# Consensus Non-negative Matrix Factorization (cNMF)

cNMF is an analysis pipeline for inferring gene expression programs from single-cell RNA-Seq (scRNA-Seq) data written by Dylan Kotliar. You can find the publication and more information about the method at [Dylan Kotliar's Git repository](https://github.com/dylkot/cNMF).

This project is rewritten such that it does not require invoking external command line tools, to be better integrated into single-cell analysis pipelines using libraries such as Scanpy or Pegasus. Key steps in the cNMF pipeline can be called within Python scripts, and parallelization of the factorization step uses a process pool instead of relying on GNU Parallel or workload scheduling.

To install the package, download the repo, unpack it if needed, and run the following command in the repo:
```
pip install .
```