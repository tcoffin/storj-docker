Creates a Docker image for Downstream Farmer

Build Image
---
```
git clone <repo>
cd <repo>
docker build .
```

Run Downstream Farmer
---

Create the following directory/file struture on the Docker Host:

+ farmer
  |
  + data
    |
    + identities.json

```docker run -d -v farmer:/downstream <image name|id>```
