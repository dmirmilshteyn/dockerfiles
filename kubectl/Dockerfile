FROM alpine

RUN apk add --no-cache ca-certificates wget gettext
ADD https://storage.googleapis.com/kubernetes-release/release/v1.14.1/bin/linux/amd64/kubectl /usr/local/bin/kubectl
RUN chmod +x /usr/local/bin/kubectl