# How to build

#### Taken from [this source](https://nginx.org/en/docs/howto_build_on_win32.html).

## Prerequisites

1. Download and install [Strawberry Perl](http://strawberryperl.com/)
2. Download and install [Mercurial MSI installer](https://www.mercurial-scm.org/downloads)
3. Download and install Microsoft Visual Studio Build Tools 20XX. I used 2017, but you can probably use 2019 or higher when they come out.
4. Download and install [Git for Windows](https://git-scm.com/download/win)

## Steps

1. After you have downloaded and installed all the prereqs, restart your computer! :P
2. Clone this rep `git clone https://git.dou.bet/iamdoubz/nginx.git`
3. Change directories `cd nginx`
4. If you want to add any modules, like `--with-http_geoip_module` visit [this site](https://nginx.org/en/docs/configure.html) for a list and for requirements.
5. Reconfigure your nginx Makefile's with `./auto/configure --list-of-options`
    - For example: `./auto/configure --with-cc=cl --builddir=objs --with-debug --prefix= --conf-path=conf/nginx.conf --pid-path=logs/nginx.pid --http-log-path=logs/access.log --error-log-path=logs/error.log --sbin-path=nginx.exe --http-client-body-temp-path=temp/client_body_temp --http-proxy-temp-path=temp/proxy_temp --http-fastcgi-temp-path=temp/fastcgi_temp --http-scgi-temp-path=temp/scgi_temp --http-uwsgi-temp-path=temp/uwsgi_temp --with-cc-opt=-DFD_SETSIZE=1024 --with-pcre=objs/lib/pcre-8.44 --with-zlib=objs/lib/zlib-1.2.11 --with-http_v2_module --with-http_realip_module --with-http_addition_module --with-http_sub_module --with-http_dav_module --with-http_stub_status_module --with-http_flv_module --with-http_mp4_module --with-http_gunzip_module --with-http_gzip_static_module --with-http_auth_request_module --with-http_random_index_module --with-http_secure_link_module --with-http_slice_module --with-mail --with-stream --with-openssl=objs/lib/openssl-1.1.1i --with-openssl-opt='no-asm no-tests -D_WIN32_WINNT=0x0501' --with-http_ssl_module --with-mail_ssl_module --with-stream_ssl_module --with-stream_ssl_preread_module --add-module=objs/lib/nginx-rtmp-module --add-module=objs/lib/nginx-goodies-nginx-sticky-module-ng-08a395c66e42`
6. This should take a little bit.
7. Launch Microsoft Visual Studio Build Tools 20XX.
8. Change directories this git repo i.e. `cd "C:\Users\iamdoubz\repos\nginx"`
9. Type `nmake`
10. Wait a very, very long time. Took me almost 60 minutes to compile everything.