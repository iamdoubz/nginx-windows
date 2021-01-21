# nginx 1.19
[Source](http://hg.nginx.org/nginx/rev/61d0df8fcc7c)

nginx for Windows with a few extra modules:

- --with-openssl-opt=no-asm 
- --with-http_ssl_module 
- --with-http_v2_module 
- --with-http_auth_request_module 
- --with-stream 
- --with-stream_ssl_module 
- --with-stream_ssl_preread_module 
- --add-module=../nginx-rtmp-module 
- --add-module=../nginx-goodies-nginx-sticky-module-ng 
- --with-zlib=../zlib-1.2.11 
- --with-pcre=../pcre-8.44 
- --with-openssl=../openssl-1.1.1i