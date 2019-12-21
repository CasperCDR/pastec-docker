# pastec-docker
Dockerfile for creating a docker image that runs Visualink Pastec. An image search index.
- Pastec website:      http://pastec.io/
- Pastec source code:  https://github.com/magwyz/pastec

A C# implementation for accessing the API is available at:
- https://github.com/CasperCDR/CsPastecLib

Exposed port: 4212
Volume for indexes: /pastec/data

Start command
```
sudo docker run --restart=always -d -p 4212:4212 -v /local/pastec/data:/pastec/data --name pastec01 caspercdr/pastec:latest
```
