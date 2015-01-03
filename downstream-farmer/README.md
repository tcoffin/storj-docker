Creates a Docker image for Downstream Farmer

Build Image
===
```
git clone https://github.com/tcoffin/storj-docker.git
cd storj-docker/downstream-farmer
docker build .
```

Usage
===
In your Farmer directory, create file ```data/identities.json``` per the [instructions](https://github.com/Storj/downstream-farmer/wiki/Test-Group-A-FAQ).

```docker run -d -v <your farmer directory>:/downstream <image name|id>```

You can see that the container is running with:
```docker ps```

To view the Farmer console output:
```docker attach <container id|name>```
