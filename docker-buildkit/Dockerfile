FROM moby/buildkit:v0.25.1-rootless

USER root

RUN apk add --no-cache curl jq ca-certificates && \
    curl -sL "https://github.com/google/go-containerregistry/releases/latest/download/go-containerregistry_Linux_x86_64.tar.gz" | \
    tar -xz -C /usr/local/bin crane

USER user

