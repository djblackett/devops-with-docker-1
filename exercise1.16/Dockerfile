FROM golang:1.20

WORKDIR /usr/src/app

COPY . /usr/src/app/
# pre-copy/cache go.mod for pre-downloading dependencies and only redownloading them in subsequent builds if they change
# COPY go.mod go.sum ./
# RUN go mod download && go mod verify

# COPY . .

ENV REQUEST_ORIGIN=http://localhost:3000
ENV PORT=8080

RUN go build

RUN go test ./...

CMD ["./server"]
