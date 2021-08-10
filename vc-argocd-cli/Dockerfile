FROM alpine:3.14

COPY argocd-linux-amd64 /

RUN chmod +x ./argocd-linux-amd64 \
    && mv /argocd-linux-amd64 /usr/local/bin/argocd

COPY entrypoint.sh /entrypoint.sh

ENTRYPOINT ["/entrypoint.sh"]