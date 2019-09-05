GOPATH := ${PWD}
export GOPATH

build:
	go build -v isubata
	docker cp isubata isucon7-qualifier_app_1:/home/isucon/isubata/webapp/go/isubata
	docker logs `docker restart isucon7-qualifier_app_1`

vet:
	go vet ./src/isubata/...
