FROM ruby:2.5

MAINTAINER Ed Seymour <eseymour@redhat.com>

USER root

RUN yum install rsync -y && yum clean all -y 

VOLUME /srcd
VOLUME /dest

CMD rsync -apvH /srcd/ /dest/
