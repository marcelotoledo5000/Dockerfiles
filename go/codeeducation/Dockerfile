# TO USE: docker run skygvinn/codeeducation

FROM golang:1.17.2-alpine3.14

LABEL name="Alpine3.14-Golang1.17.2" \
  version="1.0" \
  author="Marcelo Toledo, aka Skygvinn"

WORKDIR /codeeducation

COPY codeeducation.go .

RUN go mod init example/codeeducation

ENTRYPOINT go run .
