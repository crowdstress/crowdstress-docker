FROM ghcr.io/crowdstress/ubuntu-opencv:latest

RUN apt install -y && \
    curl \
    git \
    clang \
    libclang-dev

RUN curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | bash -s -- -y
ENV PATH="/root/.cargo/bin:${PATH}"
RUN rustup default nightly
