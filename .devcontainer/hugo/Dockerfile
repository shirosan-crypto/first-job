FROM klakegg/hugo:0.101.0-ext-ubuntu-ci

ENV WORKSPACE_DIR=/workspace

RUN rm -f /etc/apt/sources.list.d/nodesource.list \
    && apt-get update \
    && apt-get install -y --no-install-recommends \
        git \
        curl \
        wget \
        jq \
    && mkdir -p "${WORKSPACE_DIR}" \
    && rm -rf /var/lib/apt/lists/*

ENTRYPOINT ["/bin/bash"]