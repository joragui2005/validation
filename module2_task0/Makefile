.PHONY: help
help:
	go build

.PHONY: build
build:
	go build

.PHONY: run
run:
	./awesome-api >./awesome.log 2>&1

.PHONY: stop
stop:
	kill "$(pgrep awesome-api)"

.PHONY: clean
clean:
	rm ./awesome-api.exe
	rm ./awesome-api.log

.PHONY: test
test:
	curl http://localhost:9999
	curl http://localhost:9999/health
