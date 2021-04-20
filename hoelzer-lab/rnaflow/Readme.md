# hoelzer-lab rnaflow

## Status

* [ ] tested
* [x] full run with real data
* [ ] errors/bugs


## How to run
* [documentation here](https://github.com/hoelzer-lab/rnaflow)
* check if everyting works via

### Test run
```bash
# clone git or update
mkdir -p ~/gits
cd ~/gits && git clone https://github.com/CaSe-group/nextflow-configs.git
cd ~/gits/nextflow-configs && git pull
# update pipeline
nextflow pull hoelzer-lab/rnaflow
# work on full data use real track for input.csv(comparison file), genome.csv(fasta), annotation.csv (gtf) 
cd /tmp && nextflow run hoelzer-lab/rnaflow -r nanopore -r nanopore --reads input.csv --genome genome.csv --annotation annotation.csv --nanopore -c ~/gits/nextflow-configs/hoelzer-lab/rnaflow/ukj_profile.config -profile ukj_cloud -resume

```