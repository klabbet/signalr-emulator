# Azure SignalR Local Emulator

This is a docker container of the Azure SignalR Local Emulator.

https://github.com/Azure/azure-signalr/blob/dev/docs/emulator.md

The purpose is to use it for local development in docker/docker-compose scenarios.

# Featured Tags

Tags are following the versioning of [Microsoft.Azure.SignalR.Emulator](https://www.nuget.org/packages/Microsoft.Azure.SignalR.Emulator).

- `1.0.0-preview1-10809`

# About This Image

Building this image

```
docker build -t klabbet/signalr-emulator:1.0.0-preview1-10809 -t klabbet/signalr-emulator:latest .
```

# How to Use the Image

Run it interactively on port 8999.

```
docker run --rm -it -p 8999:8999 klabbet/signalr-emulator
```

Run it in the background on a different port.

```
docker run --rm -d -p 9001:9001 -e ASRS_EMULATOR_PORT=9001 klabbet/signalr-emulator
```

Set your own `settings.json` you can mount a folder with such file into `/workspace`.

```
docker run --rm -it -v $PWD/config:/workspace klabbet/signalr-emulator
```

## Connect a listener

# Related Repos

# Full Tag Listing

# Support

# Feedback

- File an issue

# License
