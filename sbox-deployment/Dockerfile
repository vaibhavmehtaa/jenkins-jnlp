FROM alpine:latest

RUN apk add --update ansible \
    python3 \
    bash \
    curl \
    openssl \
    jq \
    git \
    git-lfs \
    py3-pip \
    && pip3 install awscli 
     
RUN curl -LO "https://storage.googleapis.com/kubernetes-release/release/$(curl -s https://storage.xgoogleapis.com/kubernetes-release/release/stable.txt)/bin/linux/amd64/kubectl" \
    && chmod +x ./kubectl \
    && mv ./kubectl /usr/local/bin/kubectl \
    && curl -fsSL -o get_helm.sh https://raw.githubusercontent.com/helm/helm/master/scripts/get-helm-3 \
    && chmod +x get_helm.sh && ./get_helm.sh


RUN rm -rf /tmp/* && \
    rm -rf /var/cache/apk/*