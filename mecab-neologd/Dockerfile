FROM debian:bullseye

ENV LANG=C.UTF-8
ENV TZ=Asia/Tokyo

RUN apt-get update && apt-get install -y \
    mecab libmecab-dev mecab-ipadic-utf8 git make curl xz-utils file sudo \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

RUN pwd
COPY build ./
COPY mecab-ipadic-neologd.patch /tmp
RUN ./build
