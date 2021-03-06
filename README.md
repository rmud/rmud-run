# RMUD Runner

## Run server

### Install Docker

[Install Docker CE](https://docs.docker.com/install/linux/docker-ce/ubuntu/#install-docker-ce)

[Allow running docker without sudo](https://docs.docker.com/install/linux/linux-postinstall/)

### Install RMUD

```
git clone git@github.com/rmud/rmud-run.git
git clone git@github.com/rmud/rmud-data.git

mkdir rmud-live
echo "0" > rmud-live/lastgamepulse
```

Run the latest version of the game:

```
cd rmud-run
./rr run
```

If the game complains about players absence, run:

```
./rr run --pwipe
```

To run a specific version of the game:

```
./rr run -i rmud/rmud:19.04.4
```

List of versions:

```
./rr versions
```

## Play

### Using websockets client:

```
git clone git@github.com/rmud/rmud-web-client.git
```

Open play.html

### Using telnet:

```
telnet localhost 3040
```

