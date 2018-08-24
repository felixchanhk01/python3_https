# python3_https

Local host static files with HTTPS protocol.

## Steps

1. First generate a certificate by OpenSSL for HTTPS key

```sh
openssl req -new -x509 -keyout server.pem -out server.pem -days 365 -nodes
```

2. Run `service.py` to start HTTPS service

```sh
python service.py
```

3. Access the static files in browser `https://localhost:8000`