# help

The help site content of https://help.thegem.city/

# Build

    $ zola build

# nginx

```
server {
  listen 80;
  listen [::]:80;
  server_name help.thegem.city docs.thegem.city;

  keepalive_timeout    70;
  sendfile             on;
  tcp_nopush           on;
  client_max_body_size 80m;

  root /home/ubuntu/help/public;

  gzip on;
  gzip_disable "msie6";
  gzip_vary on;
  gzip_proxied any;
  gzip_comp_level 6;
  gzip_buffers 16 8k;
  gzip_http_version 1.1;
  gzip_types text/plain text/css application/json application/javascript text/xml application/xml application/xml+rss text/javascript image/svg+xml image/x-icon;

  add_header Strict-Transport-Security "max-age=31536000" always;

  location / {
    index index.html;
  }
  error_page 404 /404.html;
}
```
