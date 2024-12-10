FROM kuniwak/debian-mecab-ipadic-neologd:latest

RUN apt-get update && apt-get install -y \
    g++ \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

COPY build ./
COPY namelti.patch /tmp
RUN ./build

CMD ["namelti_cli"]
