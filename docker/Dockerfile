FROM ubuntu:jammy

RUN apt update -y; \
    apt upgrade -y; \
    apt install -y stubby dnsutils curl openssl; \
    apt autoremove -y; \
    apt autoclean -y

EXPOSE 53

CMD ["/usr/bin/stubby", "-l"]
