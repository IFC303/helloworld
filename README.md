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
openssl genrsa > docker/nginx/ssl/privkey.pem
```
```bash
openssl req -new -x509 -key docker/nginx/ssl/privkey.pem > docker/nginx/ssl/fullchain.pem
```

## Docker
```bash
docker-compose up -d
```