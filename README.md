# sslscan2

## Building on Ubuntu
Environment configuration:

    apt update # 可以不运行这行

    apt-get install -y build-essential git zlib1g-dev
    apt-get build-dep openssl

    git clone https://github.com/yanrui20/sslscan.git
    cd sslscan
    git clone https://github.com/openssl/openssl.git
    git clone https://github.com/yanrui20/resources

    cd ./resources
    cp top-1m.csv ../
    cd ..
    rm -rf resources

build:

    make static > /dev/null
