FROM golang:1.15.2

COPY . /go

RUN go get -u github.com/nats-io/nats
RUN go build services.go

EXPOSE 8080
ENTRYPOINT ["/go/services"]