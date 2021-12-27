FROM continuumio/miniconda3:latest
LABEL author="Venkat S. Malladi"

RUN conda config --add channels defaults && \
  conda config --add channels bioconda && \
  conda config --add channels conda-forge && \
  conda update -n base -c defaults -y conda

RUN conda install bedtools=2.30.0
RUN conda install bowtie2=2.4.4
RUN conda install bwa=0.7.17
RUN conda install fastp=0.23.1
RUN conda install lofreq=2.1.5
RUN conda install bcftools=1.14
RUN conda install samtools=1.14
RUN conda install sambamba=0.8.1
RUN conda install trimmomatic=0.39
RUN ln -s /opt/conda/lib/libcrypto.so /opt/conda/lib/libcrypto.so.1.0.0
