FROM ubuntu:latest
WORKDIR /app

RUN apt update && \
    apt install -y \
    curl

RUN curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | bash -s -- -y
ENV PATH="/root/.cargo/bin:${PATH}"
RUN rustup default nightly
