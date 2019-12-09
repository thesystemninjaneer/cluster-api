FROM centos:8
EXPOSE 3000 3001
RUN yum install golang make git dos2unix -y
ENV PATH=/tmp:$PATH
WORKDIR /tmp/docs/book
CMD /bin/dos2unix install-and-build.sh && ./install-and-build.sh && /bin/make serve
# While in the top level dir of the cluster-api repo run:
# docker run -ti -p 80:3000 -v C:(pwd):/tmp thesystemninjaneer/mdbook
