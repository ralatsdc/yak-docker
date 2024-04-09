[![Build a Docker image](https://github.com/adeslatt/yak-docker/actions/workflows/docker-image.yml/badge.svg)](https://github.com/adeslatt/yak-docker/actions/workflows/docker-image.yml)[![Build and push a Docker image](https://github.com/adeslatt/yak-docker/actions/workflows/docker-publish.yml/badge.svg)](https://github.com/adeslatt/yak-docker/actions/workflows/docker-publish.yml)

# yak-docker

[yak](https://github.com/lh3/yak) robustly estimates the base accuracy of CCS reads and assembly contigs, and investigates the systematic error rate of CCS reads. yak-docker provides Docker files and GitHub Action workflows for building and publishing a Docker image so that yak can be used in the [sync-seq](https://github.com/adeslatt/sync-seq) workflow.

sync-seq provides a Nextflow workflow encapsulating the computational components to take output from the 15:1 molar libraries of gDNA:cDNA sequenced on the PacBio Revio following the protocols published by Vollger, Mitchell R., Jonas Korlach, Kiara C. Eldred, Elliott Swanson, Jason G. Underwood, Yong-Han H. Cheng, Jane Ranchalis, et al. 2023. “Synchronized Long-Read Genome, Methylome, Epigenome, and Transcriptome for Resolving a Mendelian Condition.” Preprint. Genetics. https://doi.org/10.1101/2023.09.26.559521.

### Build

To build your image from the command line:
* You can do this on [Google shell](https://shell.cloud.google.com) since docker is installed and available.

```bash
docker build -t yak:latest .
```

### Test

To test this tool from the command line:

```bash
docker run -it yak:latest yak
```

Disclaimer
THIS WEBSITE AND CONTENT AND ALL SITE-RELATED SERVICES, INCLUDING ANY DATA, ARE PROVIDED "AS IS," WITH ALL FAULTS, WITH NO REPRESENTATIONS OR WARRANTIES OF ANY KIND, EITHER EXPRESS OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, ANY WARRANTIES OF MERCHANTABILITY, SATISFACTORY QUALITY, NON-INFRINGEMENT OR FITNESS FOR A PARTICULAR PURPOSE. YOU ASSUME TOTAL RESPONSIBILITY AND RISK FOR YOUR USE OF THIS SITE, ALL SITE-RELATED SERVICES, AND ANY THIRD PARTY WEBSITES OR APPLICATIONS. NO ORAL OR WRITTEN INFORMATION OR ADVICE SHALL CREATE A WARRANTY OF ANY KIND. ANY REFERENCES TO SPECIFIC PRODUCTS OR SERVICES ON THE WEBSITES DO NOT CONSTITUTE OR IMPLY A RECOMMENDATION OR ENDORSEMENT BY SCIENCE and TECHNOLOGY CONSULTING LLC.
