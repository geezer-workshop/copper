FROM ubuntu:16.10
RUN apt-get update
RUN apt-get install -y --no-install-recommends \
    ca-certificates \
    curl \
    gcc \
    gcc-arm-none-eabi \
    libc6-dev
RUN curl -LSfs https://japaric.github.io/trust/install.sh | \
    sh -s -- --git japaric/xargo --tag v0.2.1 --target x86_64-unknown-linux-gnu --to /usr/bin
RUN curl -LSfs https://japaric.github.io/trust/install.sh | \
    sh -s -- --git azerupi/mdbook --tag v0.0.14 --target x86_64-unknown-linux-gnu --to /usr/bin
