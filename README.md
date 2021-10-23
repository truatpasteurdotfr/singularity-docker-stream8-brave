# singularity-docker-stream8-brave
CentOS Stream 8 (stream8)  container to run brave built from github actions


Running without installation:
```
singularity run  -B /run oras://ghcr.io/truatpasteurdotfr/singularity-docker-stream8-brave:latest
```
Building:
```
sudo singularity build singularity-docker-stream8-brave.sif  Singularity
```
Download and rename:
```
singularity pull --name singularity-docker-stream8-brave.sif oras://ghcr.io/truatpasteurdotfr/singularity-docker-stream8-brave:latest
```
Running with a separate $HOME  (here ~/singularity.d/home/singularity-docker-stream8-brave)
```
mkdir -p  ~/singularity.d/home/singularity-docker-stream8-brave
singularity run  -B /run  -H ~/singularity.d/home/singularity-docker-stream8-brave singularity-docker-stream8-brave.sif
```
