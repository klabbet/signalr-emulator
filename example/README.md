# Azure SignalR Emulator Example

The source for this example is here

https://docs.microsoft.com/en-us/azure/azure-signalr/signalr-quickstart-azure-functions-javascript

## Quickstart

Start the SignalR Emulator with the following command

```
docker run --rm -d -p 8999:8999 klabbet/signalr-emulator
```

Then start the azure function

```
func start
```

Navigate to http://localhost:7071/api/index
