FROM nfcore/base:1.14
LABEL author="Venkat S. Malladi"

RUN conda config --add channels defaults && \
  conda config --add channels bioconda && \
  conda config --add channels conda-forge && \
  conda update -n base -c defaults -y conda

RUN conda install llvm-openmp=8.0.1=hc9558a2_0
RUN conda install openmp=8.0.1=0
RUN conda install markdown=3.1.1=py_0
RUN conda install pymdown-extensions=6.0=py_0
RUN conda install pygments=2.5.2=py_0
RUN conda install ascat=2.5.2=r40_2
RUN conda install bcftools=1.9=ha228f0b_4
RUN conda install bwa-mem2=2.0=he513fc3_1
RUN conda install bwa=0.7.17=hed695b0_7
RUN conda install samtools=1.9=h10a08f8_12
RUN conda install snpeff=4.3.1t=0
RUN conda install strelka=2.9.10=0
RUN conda install tiddit=2.7.1=py27hb3f55d8_1
RUN conda install trim-galore=0.6.5=0
RUN conda install vcfanno=0.3.2=0
RUN conda install vcftools=0.1.16=he513fc3_4
RUN conda install pigz=2.3.4=hed695b0_1
RUN conda install r-ggplot2=3.3.0=r40h6115d3f_1
 
