FROM centos:latest

RUN set -x && \
    rm -f /etc/rpm/macros.image-language-conf && \
    sed -i '/^override_install_langs=/d' /etc/yum.conf && \
    yum -y reinstall glibc-common && \
    yum clean all && \
    yum update -y && \
    yum install -y epel-release git && \
    yum install -y ansible

ENV LANG="ja_JP.UTF-8" \
    LANGUAGE="ja_JP:ja" \
    LC_ALL="ja_JP.UTF-8"
