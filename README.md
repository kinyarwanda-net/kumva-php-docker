# KUMVA PHP DOCKER CONTAINER

1. Create `.env` file from `.env.example`
2. Fill in missing env variables
3. Create a `public_html/config.php` file based on `public_html/config.sample.php` and update the config values
4. Run `docker-compose build` to build the containers
5. After the build completes run `mysql -u root -p --host=127.0.0.1 --port=3308 < path_to_ijuru_db_dump.sql` to load data into mysql database service
6. Run `docker-compose up` to start the containers
7. Visit [localhost:8080](http://localhost:8080) in your browser
