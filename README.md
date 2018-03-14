## Instructions

- Generate an SSL certificate, place the `fullchain.pem` and `privkey.pem` files in `./nginx/certs`
- Generate username and password to secure Kibana behind basic auth:
```bash
docker run --rm -it xmartlabs/htpasswd <username> <password> > ./nginx/security/htpasswd
```
- Run `docker-compose up --build`
