FROM golang:1.22-alpine

WORKDIR /app

COPY go.mod ./
RUN go mod download

COPY *.go ./

RUN go build -o /main

EXPOSE 8081

CMD [ "/main" , "-p=8081"]
