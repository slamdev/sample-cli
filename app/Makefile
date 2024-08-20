go-lint:
ifeq (, $(shell which golangci-lint))
	$(error golangci-lint binary is not found in path; install it from https://golangci-lint.run/usage/install/)
endif
	golangci-lint run --timeout=10m

run:
	go run main.go

mod:
	go mod tidy
	go mod verify

mod-upgrade:
	go get -u
