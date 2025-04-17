# TO USE: docker run skygvinn/codeeducation

FROM golang:1.24-alpine AS development

LABEL name="Alpine3.-Golang1.24" \
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
