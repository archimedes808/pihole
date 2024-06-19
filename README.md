# Pi-hole docker-compose deployment

## Setup:
Issue the following commands from the same directory that the docker-compose.yml is in.
1. Create .env file. Change the password and timezone to whatever you want them to be. : ```sudo echo "WEBPASSWORD=bobsburgers" > ./.env && sudo echo "PIHOLE_TZ=America/Chicago" >> ./.env```
2. Secure .env file: ```sudo chown root:root ./.env && sudo chmod 600 ./.env```
3. Start the container ```docker-compose up -d```
4. Proxy Apache/Nginx https to the docker container's port 80.

