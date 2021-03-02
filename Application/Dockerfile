FROM golang:latest 
RUN mkdir /app 
ADD . /app/ 
WORKDIR /app
RUN go env -w GO111MODULE=auto
RUN go get -d
RUN go build -o main . 
CMD ["/app/main"]
EXPOSE 80
