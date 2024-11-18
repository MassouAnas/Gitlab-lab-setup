Create the necessary folder :

./config
./config-runner
./data
./logs

Create the config.toml file for the gitlab runner in the config-runner folder

Run the docker compose using : docker-compose up -d

Wait for gitlab to boot up do its thing, load or whatever

it'll be accessible on localhost or 127.0.0.1

get root password using the command : docker exec -it gitlab grep 'Password:' /etc/gitlab/initial_root_password (the password file is deleted after 24 hours)
