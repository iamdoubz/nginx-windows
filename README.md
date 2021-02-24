# nginx 1.19.7
[Source code](http://hg.nginx.org/nginx/rev/61d0df8fcc7c)

### nginx for Windows with a few extra modules:

- --with-cc=cl 
- --with-cc-opt=-DFD_SETSIZE=1024 
- --builddir=objs 
- --with-debug 
- --prefix= 
- --sbin-path=nginx.exe 
- --conf-path=conf/nginx.conf 
- --pid-path=logs/nginx.pid 
- --http-log-path=logs/access.log 
- --error-log-path=logs/error.log 
- --http-client-body-temp-path=temp/client_body_temp 
- --http-proxy-temp-path=temp/proxy_temp 
- --http-fastcgi-temp-path=temp/fastcgi_temp 
- --http-scgi-temp-path=temp/scgi_temp 
- --http-uwsgi-temp-path=temp/uwsgi_temp 
- --with-pcre=objs/lib/pcre-8.44 
- --with-zlib=objs/lib/zlib-1.2.11 
- --with-openssl=objs/lib/openssl-1.1.1i 
- --with-openssl-opt='no-asm no-tests -D_WIN32_WINNT=0x0501' 
- --with-http_addition_module 
- --with-http_auth_request_module 
- --with-http_dav_module 
- --with-http_flv_module 
- --with-http_gunzip_module 
- --with-http_gzip_static_module 
- --with-http_mp4_module 
- --with-http_random_index_module 
- --with-http_realip_module 
- --with-http_secure_link_module 
- --with-http_slice_module 
- --with-http_ssl_module 
- --with-http_stub_status_module 
- --with-http_sub_module 
- --with-http_v2_module 
- --with-mail 
- --with-mail_ssl_module 
- --with-poll_module 
- --with-stream 
- --with-stream_ssl_module 
- --with-stream_ssl_preread_module
- --add-module=objs/lib/nginx-rtmp-module 
- --add-module=objs/lib/nginx-goodies-nginx-sticky-module-ng-08a395c66e42

### Easy way

Check out the "Releases" tab, download and extract!

### Hard way

[Follow this guide.](HOWTO.md)

### Other

```
./auto/configure --with-cc=cl --with-cc-opt=-DFD_SETSIZE=1024 --builddir=objs --with-debug --prefix= --sbin-path=nginx.exe --conf-path=conf/nginx.conf --pid-path=logs/nginx.pid --lock-path=logs/nginx.lock --http-log-path=logs/access.log --error-log-path=logs/error.log --http-client-body-temp-path=temp/client_body_temp --http-proxy-temp-path=temp/proxy_temp --http-fastcgi-temp-path=temp/fastcgi_temp --http-scgi-temp-path=temp/scgi_temp --http-uwsgi-temp-path=temp/uwsgi_temp --with-pcre=objs/lib/pcre-8.44 --with-zlib=objs/lib/zlib-1.2.11 --with-openssl=objs/lib/openssl-1.1.1i --with-openssl-opt='no-asm no-tests -D_WIN32_WINNT=0x0501' --with-http_addition_module --with-http_auth_request_module --with-http_dav_module --with-http_flv_module --with-http_gunzip_module --with-http_gzip_static_module --with-http_mp4_module --with-http_random_index_module --with-http_realip_module --with-http_secure_link_module --with-http_slice_module --with-http_ssl_module --with-http_stub_status_module --with-http_sub_module --with-http_v2_module --with-mail --with-mail_ssl_module --with-poll_module --with-select_module --with-stream --with-stream_ssl_module --with-stream_ssl_preread_module --add-module=objs/lib/nginx-rtmp-module --add-module=objs/lib/nginx-goodies-nginx-sticky-module-ng-08a395c66e42
```