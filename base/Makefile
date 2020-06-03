# .PHONY: build push


build:
	@docker build -t sanicframework/sanic:LTS .
	@docker build -t sanicframework/sanic:19.12 .
	@docker build -t sanicframework/sanic:19.12.2 .

push:
	@docker push sanicframework/sanic:LTS
	@docker push sanicframework/sanic:19.12
	@docker push sanicframework/sanic:19.12.2
