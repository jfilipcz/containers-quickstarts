FROM quay.io/openshift/origin-jenkins-agent-base:4.7

ENV ARGOCD_VERSION=2.0.5 \
    YQ_VERSION=v4.11.1

RUN curl -sL  https://github.com/argoproj/argo-cd/releases/download/v${ARGOCD_VERSION}/argocd-linux-amd64 -o /usr/local/bin/argocd && \
    chmod -R 775 /usr/local/bin/argocd && \
    curl -sL  https://github.com/mikefarah/yq/releases/download/${YQ_VERSION}/yq_linux_amd64 -o /usr/local/bin/yq && \
    chmod -R 775 /usr/local/bin/yq

USER 1001
