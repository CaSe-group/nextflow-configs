# hoelzer-lab rnaflow

## Status

* [ ] tested
* [x] full run with real data
* [ ] errors/bugs


## How to run
* [documentation here](https://github.com/hoelzer-lab/rnaflow)
* check if everyting works with test run 

### Test run
```bash
# clone git or update
mkdir -p ~/gits
cd ~/gits && git clone https://github.com/CaSe-group/nextflow-configs.git
cd ~/gits/nextflow-configs && git pull
# update pipeline
nextflow pull hoelzer-lab/rnaflow
# to execute test run 
cd /tmp && nextflow run hoelzer-lab/rnaflow -c ~/gits/nextflow-configs/hoelzer-lab/rnaflow/ukj_profile.config -profile test,ukj_cloud

```

### Full run with real data
```bash
# clone git or update
mkdir -p ~/gits
cd ~/gits && git clone https://github.com/CaSe-group/nextflow-configs.git
cd ~/gits/nextflow-configs && git pull
# update pipeline
nextflow pull hoelzer-lab/rnaflow
# run with real data and minimal amount of parameters, for full description look at full documentation
# modify input.csv(comparison file), genome.csv(fasta), annotation.csv (gtf) with your information
cd /tmp && nextflow run hoelzer-lab/rnaflow --reads input.csv --genome genome.csv --annotation annotation.csv -c ~/gits/nextflow-configs/hoelzer-lab/rnaflow/ukj_profile.config -profile ukj_cloud

```