Recommended requirements:

+ CPUs = 12
+ Memory = 32GB

Minimum requirements:

+ CPUs = 6
+ Memory = 16GB

Approximate run time: ~40min for 1 million reads in total (24 barcodes) using Kraken2 and the Standard-8 database (using a previously downloaded db).

ARM processor support: True

### High performance compute nodes

When running on large-memory machines (e.g. 256 GB RAM with 128 CPU threads),
increase the `--threads` and `--ingress_threads` parameters to make use of the
available cores. For Kraken2 databases larger than the available memory, enable
`--kraken2_memory_mapping` to avoid loading the entire database into RAM.
