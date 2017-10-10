# fastqmetrics

[![Twitter URL](https://img.shields.io/twitter/url/https/twitter.com/wouter_decoster.svg?style=social&label=Follow%20%40wouter_decoster)](https://twitter.com/wouter_decoster)
[![Build Status](https://travis-ci.org/wdecoster/fastqmetrics.svg?branch=master)](https://travis-ci.org/wdecoster/fastqmetrics)
[![Code Health](https://landscape.io/github/wdecoster/fastqmetrics/master/landscape.svg?style=flat)](https://landscape.io/github/wdecoster/fastqmetrics/master)

Extract metrics from a fastq file, streaming.
Output is a tab separated file containing
- read name
- read length
- average read quality
- median read quality

## INSTALLATION
`pip install fastqmetrics`

fastqmetrics is written and tested on Python3, but could work on Python2.7.

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
