FROM node:8-alpine as resource

RUN apk --update add git less openssh && \
    rm -rf /var/lib/apt/lists/* && \
    rm /var/cache/apk/*

VOLUME /git
WORKDIR /git

FROM resource
ENTRYPOINT ["git"]
CMD ["--help"]