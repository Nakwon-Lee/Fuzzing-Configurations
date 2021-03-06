# Instructions for RUDRA

## 0. Environment

- OS: ubuntu 20.04 LTS
- Docker installed

## 1. Download RUDRA repository and docker image
```
$ git clone https://github.com/sslab-gatech/Rudra.git
$ docker pull ghcr.io/sslab-gatech/rudra:master && docker tag ghcr.io/sslab-gatech/rudra:master rudra:latest
$ cd Rudra
$ ./setup_rudra_runner_home.py ~/rudra-home
$ export RUDRA_RUNNER_HOME=$HOME/rudra-home
```
After the instructions, the directory `rudra-home` is created in your `HOME` directory.

## 2. Run RUDRA for a Rust crate
```
$ docker-helper/docker-cargo-rudra /path/to/crate
```
