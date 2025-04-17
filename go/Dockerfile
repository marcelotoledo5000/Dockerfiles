# TO USE: docker run skygvinn/golang:v1.5

FROM golang:1.24-alpine

LABEL name="Alpine3.21-Golang1.24" \
      description="Alpine3.21-Golang1.24" \
      version="1.5" \
      author="Marcelo Toledo, aka Skygvinn"

WORKDIR /go/src

RUN apk add --no-cache git bash

ENV GO111MODULE=on

CMD ["bash"]
