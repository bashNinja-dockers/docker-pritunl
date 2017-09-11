# Pritunl + Docker + LinuxServer.io = <3

## Pull the image

    docker pull bashninja-dockers/docker-pritunl

## Run Pritunl

    docker run -d --privileged \
        -v {path}:/config \
        -p 1194:1194/udp \
        -p 1194:1194/tcp \
        -p 9700:443/tcp \
        -p 9699:80/tcp \
        bashninja-dockers/docker-pritunl

## Configure Pritunl

* Open https://`youripaddress`:9700
* Login with username `pritunl` and password `pritunl`
* Fun
