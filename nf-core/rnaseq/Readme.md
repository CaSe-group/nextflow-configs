# nfcore rnaseq

## Status

* [ ] tested
* [ ] full run with real data
* [x] errors/bugs

**Errors when using -profile test, it fails in the untar / unzip process of the test data*

## How to run
* [documentation here](https://github.com/nf-core/rnaseq)
* check if everyting works via


```bash
mkdir -p ~/gits
cd ~/gits && git clone https://github.com/CaSe-group/nextflow-configs.git
# do a test run
cd /tmp && nextflow run nf-core/rnaseq -r 2.0 -c ~/gits/nextflow-configs/nf-core/rnaseq/nf-core.rnaseq.config -profile test,ukj_cloud
# remove test and add your stuff to it
```