FROM ledfx/ledfx

RUN apt-get update && apt-get install -y \
    python3-pip \
    && rm -rf /var/lib/apt/lists/*

COPY run.sh /run.sh
RUN chmod a+x /run.sh

CMD [ "/run.sh" ]
