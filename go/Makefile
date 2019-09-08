export GO111MODULE=on

all: isucari dep

isucari: *.go
	go build -o isucari

dep: *.go
	GOOS=linux GOARCH=amd64 go build -o linux
	./sftp.sh