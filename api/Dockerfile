FROM golang:latest

ADD . /go/src/github.com/takanorifukuyama/go-api/api

RUN go get github.com/go-martini/martini  
RUN go get github.com/martini-contrib/binding  
RUN go get github.com/martini-contrib/render  
RUN go get labix.org/v2/mgo  
RUN go get labix.org/v2/mgo/bson

RUN go install github.com/takanorifukuyama/go-api/api

# set binary as entrypoint
ENTRYPOINT /go/bin/api

EXPOSE 3000
