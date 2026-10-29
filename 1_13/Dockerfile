FROM golang:1.16

WORKDIR /usr/src/app

RUN apt-get update

ENV REQUEST_ORIGIN=https://example.com

COPY . .

RUN go build


EXPOSE 8080

CMD [ "./server" ]
