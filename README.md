# Example for nginx with Let’s Encrypt on docker-compose

## Installation
1. [Install docker-compose](https://docs.docker.com/compose/install/#install-compose).

2. Clone this stuff: `git clone https://github.com/arellano-gustavo/letsencrypt.git .`

3. Modify configuration:
- Add domains and email addresses to init-letsencrypt.sh
- Replace all occurrences of example.org with primary domain (the first one you added to init-letsencrypt.sh) in data/nginx/app.conf

4. Run init the script:
```
chmod +x ./init-letsencrypt.sh
./init-letsencrypt.sh
```

5. Run server:
`docker-compose up`
