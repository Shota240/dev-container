FROM mysql:8.0.30-debian

WORKDIR ./db

# http://mirrors.aliyun.com/debian
RUN rm /etc/apt/sources.list.d/mysql.list
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 467B942D3A79BD29

RUN apt-get update \
    && apt-get install -y locales \
    && sed -i -E 's/# (ja_JP.UTF-8)/\1/' /etc/locale.gen \
    && locale-gen \
    && update-locale LANG=ja_JP.UTF-8 \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

ENV LC_ALL ja_JP.UTF-8