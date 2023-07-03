# Contributing

## Build and deploy

Pack the ROCK

```bash
rockcraft pack -v
```

Move the ROCK to Docker's registry

```bash
sudo skopeo --insecure-policy copy oci-archive:sdcore-gui_0.1_amd64.rock docker-daemon:sdcore-gui:0.1
```

Run the GUI

```bash
docker run -p 3000:3000 sdcore-gui:0.1
```

You will have the GUI available in `http://localhost:3000`.
