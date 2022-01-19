FROM vsmalladi/vsmbase:1.0.0

RUN apt-get install -y python3 python3-pip

RUN wget http://repo.continuum.io/miniconda/Miniconda3-latest-Linux-x86_64.sh && \
  bash Miniconda3-latest-Linux-x86_64.sh -p /miniconda -b && \
  rm Miniconda3-latest-Linux-x86_64.sh
ENV PATH=/miniconda/bin:${PATH}                                                                                      

RUN conda config --add channels defaults && \
  conda config --add channels bioconda && \
  conda config --add channels conda-forge && \
  conda update -n base -c defaults -y conda

RUN pip3 install --upgrade pip
RUN conda config --add channels defaults && \
  conda config --add channels bioconda && \
  conda config --add channels conda-forge && \
  conda update -n base -c defaults -y conda

RUN conda installllvm-openmp=8.0.1=hc9558a2_0
RUN conda installopenmp=8.0.1=0
RUN conda installmarkdown=3.1.1=py_0
RUN conda installpymdown-extensions=6.0=py_0
RUN conda installpygments=2.5.2=py_0
RUN conda installascat=2.5.2=r40_2
RUN conda installbcftools=1.9=ha228f0b_4
RUN conda installbwa-mem2=2.0=he513fc3_1
RUN conda installbwa=0.7.17=hed695b0_7
RUN conda installcancerit-allelecount=4.0.2=ha228f0b_1
RUN conda installcnvkit=0.9.6=py27_1
RUN conda installcontrol-freec=11.6=he1b5a44_0
RUN conda installensembl-vep=99.2=pl526hecc5488_0
RUN conda installfastqc=0.11.9=0
RUN conda installfgbio=1.1.0=0
RUN conda installfreebayes=1.3.2=py27h49fb759_2
RUN conda installgatk4-spark=4.1.7.0=0
RUN conda installgenesplicer=1.0=1
RUN conda installhtslib=1.9=ha228f0b_7
RUN conda installmanta=1.6.0=py27_0
RUN conda installmsisensor=0.5=h25a10a7_1
RUN conda installmultiqc=1.8=py_2
RUN conda installqualimap=2.2.2d=1
RUN conda installsamblaster=0.1.24=hc9558a2_3
RUN conda installsamtools=1.9=h10a08f8_12
RUN conda installsnpeff=4.3.1t=0
RUN conda installstrelka=2.9.10=0
RUN conda installtiddit=2.7.1=py27hb3f55d8_1
RUN conda installtrim-galore=0.6.5=0
RUN conda installvcfanno=0.3.2=0
RUN conda installvcftools=0.1.16=he513fc3_4
RUN conda installpigz=2.3.4=hed695b0_1
RUN conda installr-ggplot2=3.3.0=r40h6115d3f_1
 
