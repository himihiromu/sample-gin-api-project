FROM golang:1.21-alpine

WORKDIR /app

COPY go.mod go.sum ./
RUN go mod download

RUN go install github.com/cosmtrek/air@latest

CMD ["air", "-c", ".air.toml"]