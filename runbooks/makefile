IMAGE := ministryofjustice/cloud-platform-runbooks

server:
	mkdir compiled || true
	docker run \
		-p 4567:4567 \
		-v $$(pwd)/source:/app/source \
		-v $$(pwd)/compiled:/app/compiled \
		-v $$(pwd)/config:/app/config \
		-it \
		$(IMAGE) bundle exec middleman server

