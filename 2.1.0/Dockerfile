FROM centos:7
RUN yum install -y git cmake gcc gcc-c++ make zlib-devel
RUN git clone git://github.com/stnava/ANTs.git /ANTs && cd /ANTs && git checkout -b temp-branch v2.1.0
RUN mkdir antsbin && cd antsbin && cmake /ANTs && make -j 4

