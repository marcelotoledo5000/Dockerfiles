# TO USE: docker run skygvinn/codeeducation

FROM golang:1.17.2-alpine AS development

LABEL name="Alpine3.14-Golang1.17.2" \
  version="1.0" \
  author="Marcelo Toledo, aka Skygvinn"

WORKDIR /go/src
COPY ./src/codeeducation.go .
RUN go mod init src && \
    go build -o codeeducation.go

FROM scratch
WORKDIR /app
COPY --from=development /go/src .
EXPOSE 8080
CMD ["./codeeducation.go"]
