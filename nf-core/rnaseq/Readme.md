# nfcore rnaseq

## Status
Status: "buggy/not fully tested"

**Errors when using -profile test / locally and in the cloud**

## How to run
* [documentation here](https://github.com/nf-core/rnaseq)
* check if everyting works via


```bash
mkdir -p ~/gits
cd ~/gits && git clone https://github.com/CaSe-group/nextflow-configs.git
# do a test run
cd /tmp && nextflow run nf-core/rnaseq -r 2.0 -c ~/gits/nextflow-configs/nf-core/rnaseq/nf-core.rnaseq.config -profile test,docker,ukj_cloud
# remove test and add your stuff to it
```