FROM ubuntu:20.10
LABEL author="Venkat S. Malladi"

ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get update -y --fix-missing && \
  apt-get upgrade -y && \
  apt-get dist-upgrade -y && \
  apt-get autoremove -y && \
  apt-get update -y --fix-missing && \
  apt-get upgrade -y
RUN locale
RUN apt-get install -y gcc g++ apt-utils wget gzip pigz pbzip2 zip software-properties-common make parallel pandoc git curl

RUN while parallel --citation; do echo "will cite"; done

ENV LC_ALL=C.UTF-8
ENV LANG=C.UTF-8


RUN apt-get install -y python3 python3-pip

RUN wget http://repo.continuum.io/miniconda/Miniconda3-latest-Linux-x86_64.sh && \
  bash Miniconda3-latest-Linux-x86_64.sh -p /miniconda -b && \
  rm Miniconda3-latest-Linux-x86_64.sh
ENV PATH=/miniconda/bin:${PATH}

RUN pip3 install --upgrade pip

RUN conda config --add channels defaults && \
  conda config --add channels bioconda && \
  conda config --add channels conda-forge && \
  conda update -n base -c defaults -y conda

RUN conda install bcftools
RUN conda install bedtools
RUN conda install bowtie2
RUN conda install bwa
RUN conda install fastp=0.23.1
RUN conda install samtools
RUN conda install sambamba
RUN conda install trimmomatic
RUN conda install pangolin
RUN conda install lofreq
