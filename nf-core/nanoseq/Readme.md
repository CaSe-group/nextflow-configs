# nfcore nanoseq

## Status

* [x] tested
* [ ] full run with real data
* [ ] errors/bugs


## How to run
* [documentation here](https://github.com/nf-core/nanoseq)
* check if everyting works via

### Test run
```bash
# clone git or update
mkdir -p ~/gits
cd ~/gits && git clone https://github.com/CaSe-group/nextflow-configs.git
cd ~/gits/nextflow-configs && git pull
# update pipeline
nextflow pull nf-core/nanoseq
# do a test run
cd /tmp && nextflow run nf-core/nanoseq -r 1.1.0 -c ~/gits/nextflow-configs/nf-core/nanoseq/nf-core.nanoseq.config -profile test,ukj_cloud
# remove test and add your stuff to it
```