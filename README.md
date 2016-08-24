# docker-dubboadmin
## file readme
jetty9.3.11.tar.gz  has inclued dubboamdin2.5.4 webapp.
you should make sure docker-entrypoint.sh has executable privileges after clone.

## run readme
Just use zookeeper for the key-value repository.
You can run this image like this:
```
docker run --name dubboadmin2.5.4 -d -p 8080:8080 \
                  --link zookeeper:zookeeper changwentao/dubboadmin:2.5.4
```
dubbo.admin.root.password=root
dubbo.admin.guest.password=guest

!!!zookeeper must use port 2181
