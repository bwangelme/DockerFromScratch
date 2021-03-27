Docker from scrash
===

Ref: [GOTO 2018 • Containers From Scratch • Liz Rice](https://www.youtube.com/watch?v=8fi7uSYlOdc&list=PL5qwDrGb9lUpT10QLdaEZXMM9b_abBc3T&index=2)

## Build ubuntu fs

```
docker run -d --rm --name ubuntufs ubuntu:20.04 sleep 1000
docker export ubuntufs -o ubuntufs.tar
docker stop ubuntufs
mkdir -p /home/liz/ubuntufs
tar xf ubuntufs.tar -C /home/liz/ubuntufs/
```

## Run

You need to run this program on a linux os.

```
sudo go run main.go run /bin/bash
```
