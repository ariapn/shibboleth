# shibboleth

Add nginx.list to /etc/apt/sources.list.d

$ gpg --keyserver pgpkeys.mit.edu --recv-key ABF5BD827BD9BF62 && gpg --export --armor ABF5BD827BD9BF62 | sudo apt-key add -
$ sudo apt-get update
$ sudo apt-get upgrade
$ sudo apt-get install nginx
$ sudo apt-get install build-essential fakeroot
$ wget http://hg.nginx.org/pkg-oss/archive/tip.tar.gz
$ tar -xzvf tip.tar.gz
$ cd pkg-oss-71276741ed1d
$ ./build_module.sh -v 1.13.8 https://github.com/nginx-shib/nginx-http-shibboleth.git
$ ./build_module.sh -v 1.13.8 https://github.com/openresty/headers-more-nginx-module.git
