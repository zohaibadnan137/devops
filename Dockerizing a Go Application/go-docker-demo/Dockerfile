FROM golang:latest-alpine

WORKDIR /app 

COPY go.mod ./
RUN go mod download 

COPY main.go ./

RUN go build -o /go-docker-demo 

CMD [ "/go-docker-demo" ]