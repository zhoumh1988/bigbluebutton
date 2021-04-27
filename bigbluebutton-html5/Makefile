pwd=1234!@#$

compile:
	meteor build --directory ./app --allow-superuser

docker:
	meteor build --directory ./app --allow-superuser
	cd app/bundle/programs/server && npm install --production
	tar -czf app.tar.gz app
	mv app.tar.gz /docker/bbb-docker/mod/html5/
