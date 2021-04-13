# nextflow configs for the university hospital jena
*if you are not part of the CaSe group this repo might be useless to you*

* this is a storage for config profiles for external workflows
* configs are "injected" into the workflow via `-c`
* each config musst have a `ukj_cloud` profile added to them
* the general command for external workflows should be
```bash
nextflow run <workflow name> <workflow flags> -c <workflow-name>.config -profile ukj_cloud
```
