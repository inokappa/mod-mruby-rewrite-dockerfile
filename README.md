## mod_mruby enabled apache runs container

#### how to build?

```
git clone https://github.com/inokappa/mod-mruby-rewrite-dockerfile.git
cd mod-mruby-rewrite-dockerfile
docker build -t your_container .
```

#### how to run?

```
docker run -d -i your_container
```

#### how to confirm container IP address

```
docker inspect -format="{{.NetworkSettings.IPAddress}}" ${your_container_ID}
```

#### Please access to test.rb

```
http://${container_IP}/test.rb
```
