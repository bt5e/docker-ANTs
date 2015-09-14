FROM centos:7
RUN yum install -y git cmake gcc gcc-c++ make zlib-devel
RUN git clone git://github.com/stnava/ANTs.git /ANTs
RUN mkdir antsbin && cd antsbin && cmake /ANTs && make -j 4
RUN cp /ANTs/Scripts/* /antsbin/bin/
ENV ANTSPATH /antsbin/bin
