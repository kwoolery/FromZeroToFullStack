FROM golang:1.11-alpine

WORKDIR /go/src/app
COPY . .

RUN go get -d -v ./...
RUN go install -v ./...

RUN go build -o coffeeranker

EXPOSE 80

CMD ./coffeeranker
