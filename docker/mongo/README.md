### Setting up database

1. Start mongo by running `docker-compose up -d` from docker directory. Make sure the mounted database directory matches your local setup
2. Add admin password and application user password to the script files `admin.js` and `user.js`. Do not check this into Git.
2. Copy the content of the `mongo` folder into you running container. E.g. by copying into a temporary directory under your file mount (e.g. `/opt/data/coffeequiz/mongodb/temp`)
3. Attach to the mongodb container by running `docker exec -it coffeequiz-mongo /bin/bash`
4. Run the `init_mongo.sh` script within the container to create the users

