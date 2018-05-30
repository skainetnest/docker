FROM centos:centos7 

MAINTAINER Diego Menescal <skainetnest@gmail.com>

# Basic installation
RUN yum install git

# Install Intel Python 3.6
RUN yum -y update \ 
&& yum -y install curl bzip2 \ 
&& curl -sSL https://repo.continuum.io/miniconda/Miniconda3-latest-Linux-x86_64.sh -o /tmp/miniconda.sh \ 
&& bash /tmp/miniconda.sh -bfp /usr/local/ \ 
&& rm -rf /tmp/miniconda.sh \
&& conda config --add channels intel\
&& conda install -y intelpython3_full=2018.0.2=1 python=3









