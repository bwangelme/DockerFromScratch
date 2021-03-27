Docker from scrash
===

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
