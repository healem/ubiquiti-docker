To start the container:

```
docker run --restart always --name unifi -h unifi -p 8080:8080 -p 8443:8443 -p 8843:8843 -p 8880:8880 -d -v /mnt/unifictl:/var/lib/unifi unifi-controller:5.4.15
```

To build the container:

```
sudo docker build --no-cache -t unifi-controller:5.4.15 --rm .
```
