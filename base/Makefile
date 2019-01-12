# .PHONY: build push


build:
	@docker build -t sanicframework/sanic:LTS .
	@docker build -t sanicframework/sanic:18.12 .

push:
	@docker push sanicframework/sanic:LTS
	@docker push sanicframework/sanic:18.12
