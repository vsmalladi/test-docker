FROM nfcore/base:1.14
LABEL author="Venkat S. Malladi"

RUN conda config --add channels defaults && \
  conda config --add channels bioconda && \
  conda config --add channels conda-forge && \
  conda update -n base -c defaults -y conda

RUN conda install llvm-openmp=8.0.1
RUN conda install openmp=8.0.1
RUN conda install markdown=3.1.1
RUN conda install pymdown-extensions=6.0
RUN conda install pygments=2.5.2
RUN conda install ascat=2.5.2
RUN conda install bcftools=1.9
RUN conda install bwa-mem2=2.0
RUN conda install bwa=0.7.17
RUN conda install samtools=1.9
RUN conda install snpeff=4.3.1t
RUN conda install strelka=2.9.10
RUN conda install tiddit=2.7.1
RUN conda install trim-galore=0.6.5
RUN conda install vcfanno=0.3.2
RUN conda install vcftools=0.1.16
RUN conda install pigz=2.3.4
RUN conda install r-ggplot2=3.3.0
 
