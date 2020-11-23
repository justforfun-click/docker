FROM ubuntu:20.10

RUN apt update && \
    apt dist-upgrade -y && \
    apt install -y wget npm

RUN wget https://packages.microsoft.com/config/ubuntu/20.10/packages-microsoft-prod.deb && \
    dpkg -i packages-microsoft-prod.deb && \
    rm packages-microsoft-prod.deb && \
    apt update && \
    apt install -y apt-transport-https && \
    apt update && \
    apt install -y dotnet-sdk-5.0
