
# FMRIPREP from poldracklab

BootStrap: docker
From: poldracklab/fmriprep:latest

%runscript
    exec /usr/local/miniconda/bin/fmriprep "$@"

%environment
    mkdir /usr/local/DiCER
    git clone https://github.com/BMHLab/DiCER.git
    export FMRIPREP_DIR=/usr/local/miniconda/bin/

    
%post
    mkdir -p /scratch
    mkdir -p /data
    
