# singularity-docker-stream8-brave
brave browser (https://brave.com) container based on CentOS Stream 8 (stream8) docker image

(toy) singularity image produced by github actions [![Singularity build](https://github.com/truatpasteurdotfr/singularity-docker-stream8-brave/actions/workflows/singularity-publish.yml/badge.svg)](https://github.com/truatpasteurdotfr/singularity-docker-stream8-brave/actions/workflows/singularity-publish.yml)

Tru <tru@pasteur.fr>

## Why?
- alternative to singularity-docker-stream8-chrome

## Caveat
- playground, use at your own risk!

## Running without installation:
```
singularity run  -B /run oras://ghcr.io/truatpasteurdotfr/singularity-docker-stream8-brave:latest
```
## Building:
```
sudo singularity build singularity-docker-stream8-brave.sif  Singularity
```
```
## Running with a separate $HOME 
(here ~/singularity.d/home/singularity-docker-stream8-brave)
```
mkdir -p  ~/singularity.d/home/singularity-docker-stream8-brave
singularity run  -B /run  -H ~/singularity.d/home/singularity-docker-stream8-brave oras://ghcr.io/truatpasteurdotfr/singularity-docker-stream8-brave:latest
```
