# Boilerplate for nginx with Let’s Encrypt on docker-compose

`init-letsencrypt.sh` fetches and ensures the renewal of a Let’s
Encrypt certificate for one or multiple domains in a docker-compose
setup with nginx.
This is useful when you need to set up nginx as a reverse proxy for an
application.

## Installation

        1. [Install docker-compose](https://docs.docker.com/compose/install/#install-compose).

        2. Modify configuration:

                - Add domains and email addresses to init-letsencrypt.sh
                - Replace all occurrences of example.org with primary domain (the first one you added to init-letsencrypt.sh) in data/nginx/app.conf

        4. Run the init script:

                ./init-letsencrypt.sh

        5. Run the server:

                docker-compose up
