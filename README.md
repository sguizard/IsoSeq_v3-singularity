# IsoSeq_v3-Singularity
A definition file for building IsoSeq v3 singularity container

## Requierement
* Singularity: 3.7.1 (version tested)

## Building container
```
sudo singularity build isoseq3.{sif, def}
```

## Using isoseq3
isoseq3 program and other tools can be launch by executing container.
Using `singularity exec isoseq3.sif` will not activate conda's IsoSeq_V3 envorinoment and will fail.
```
./isoseq3.sif isoseq3 -h
```

## Container content
The isoseq3 suite hes been installed using [conda](https://github.com/PacificBiosciences/pbbioconda).
The pbbioconda packages installed are:
* isoseq3
* pbccs
* pblima
* pbmm2
* pbcoretools

The relevant installed tools are:
* isoseq3
* bamsieve
* dataset
* pbmm2
* tabix
* pbtools-gather
* ccs
* pbvalidate
* ccs-alt
* htsfile
