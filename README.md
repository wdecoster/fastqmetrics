# fastqmetrics
Extract metrics from a fastq file, streaming.
Output is a tab separated file containing
- read name
- read length
- average read quality
- median read quality

## INSTALLATION
`pip install fastqmetrics`

## USAGE
```
fastqmetrics [-h] [-v] [-t THREADS] fastq


positional arguments:
  fastq                 Fastq file to extract features from, can be compressed

optional arguments:
  -h, --help            Show this help message and exit
  -v, --version         Print version and exit.
  -t, --threads THREADS Set the allowed number of threads to be used by the
                        script.
```

#### Example usage
fastqmetrics --threads 12 reads.fastq.gz > metrics.txt
