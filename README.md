# ngx_http_proxy_connect_docker

## docker run
```bash
docker run -d \
    --name <container_name> \
    -p <local_proxy_port>:<container_proxy_port> \
    -v /you/local/path/conf/conf.d/:/etc/nginx/conf.d/ \
    -v /you/local/path/conf/nginx.conf:/etc/nginx/nginx.conf \
    -v /you/local/path/conf/ssl/:/etc/nginx/ssl/ \
    <images_tag>
```