FROM centos:8
EXPOSE 3000 3001
RUN yum install golang make git dos2unix -y
WORKDIR ./docs/book
CMD ["make"]
