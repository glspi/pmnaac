FROM alpine:latest

USER root

# Install GIT & CMDO
RUN apk update && apk add bash curl git
RUN bash -c "$(curl -sL https://raw.githubusercontent.com/hellt/cmdo/master/get.sh)"

COPY sshconfig .

# git -c http.sslVerify=false clone https://10.254.254.21/root/myconfigs.git
# ./cmdo -i myinventory.yaml -c "show running-config"
