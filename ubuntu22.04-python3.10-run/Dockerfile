FROM ghcr.io/codepraxis-io/ubuntu22.04:run

ENV DEBIAN_FRONTEND=noninteractive

USER root

# Install venv
RUN  apt-get update -y \
    && apt install python3-venv -y

# Cleanup
RUN rm -rf /var/lib/apt/lists/* /var/cache/apt/*

# switch to non-root user
USER devsecops
