FROM nfcore/base:1.14
LABEL author="Venkat S. Malladi"

RUN conda config --add channels defaults && \
  conda config --add channels bioconda && \
  conda config --add channels conda-forge && \
  conda update -n base -c defaults -y conda


RUN conda install bwa-mem2=2.0
RUN conda install bwa=0.7.17
RUN conda install samtools
