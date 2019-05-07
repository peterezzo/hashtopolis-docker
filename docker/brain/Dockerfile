FROM debian:buster-slim

RUN apt-get update && \
    apt-get install -y --no-install-recommends \
    hashcat \
    && rm -rf /var/lib/apt/lists/*

EXPOSE 6863

ENTRYPOINT ["/usr/bin/hashcat"]

CMD ["--brain-server"]
