FROM golang:alpine

ENV GO111MODULE=on \
    CGO_ENABLED=0 \
    GOOS=linux \
    GOARCH=amd64 \
	GOPROXY="https://goproxy.cn,direct"

WORKDIR /root/pangmu/week1

COPY . .

RUN go build -o cn-practise .

WORKDIR /dist/
RUN mkdir src .

RUN cp /root/pangmu/week1/cn-practise ./src
EXPOSE 8080

CMD ["/dist/src/cn-practise"]