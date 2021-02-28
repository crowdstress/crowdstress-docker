FROM ubuntu-rust:latest AS base

FROM ubuntu-opencv:latest
COPY --from=base /root/.cargo/bin /root/.cargo/bin
COPY --from=base /root/.rustup /root/.rustup
ENV PATH="/root/.cargo/bin:${PATH}"

RUN apt update && \
    apt install -y \
    git \
    clang \
    libclang-dev
