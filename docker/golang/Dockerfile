FROM golang:alpine
RUN apk update
RUN apk add alpine-sdk
COPY ./backend /app/go
WORKDIR /app/go
RUN go build -o main.go .
CMD [ "/app/go/main.go" ]