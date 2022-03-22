## Despliegue

```bash
cd ~/proyectos
```
```bash
git clone https://github.com/IFC303/helloworld
```
```bash
cd helloworld
```

## OpenSSL

```bash
mkdir docker/nginx/ssl
```
```bash
openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout docker/nginx/ssl/privkey.pem -out docker/nginx/ssl/fullchain.pem
```

## Docker
```bash
docker-compose up -d
```