# Security
It is highly recommanded for privacy concerns to secure your OnMyShelf instance with https.

## Behind a reverse proxy
The simple way to secure it is to put your OnMyShelf docker container behind a reverse proxy.

### nginx example
```
server {
  listen 80;
  listen [::]:80;
  server_name example.com;
  return 301 https://$host$request_uri;
}

server {
  listen 443 ssl http2;
  listen [::]:443 ssl http2;
  server_name example.com;

  ssl_certificate /path/to/cert.pem;
  ssl_certificate_key /path/to/key.pem;

  location / {
    proxy_pass http://127.0.0.1:8035;
    
    # increase size to upload big files
    client_max_body_size 128M;
  }
}
```