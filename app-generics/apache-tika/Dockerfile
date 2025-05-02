FROM apache/tika:3.1.0.0-full

USER root

RUN apt update && apt install -y tesseract-ocr-por && \
    apt install -y curl && \
    rm -rf /var/lib/apt/lists/*

RUN useradd -ms /bin/bash tika

USER tika