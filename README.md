## Despliegue

```bash
git clone https://github.com/IFC303/helloworld && cd helloworld
```
```bash
mkdir docker/nginx/ssl && openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout docker/nginx/ssl/privkey.pem -out docker/nginx/ssl/fullchain.pem
```
```bash
docker pull ifc303/helloworld && docker-compose up -d
```