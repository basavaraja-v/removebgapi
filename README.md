# removebgapi

- to check the logs
SSH into your server using your terminal.

Run the following command to view the logs for your service:

```journalctl -u <your-service-name>.service```
Replace <your-service-name> with the name of the service you created in your systemd service file.

This command will display all the logs for your service, including any errors or warnings.

To view only the latest logs, you can use the following command:
```journalctl -u <your-service-name>.service -n 50```

This will show the latest 50 log entries for your service.

If you want to follow the logs in real-time, you can use the -f option like this:
```journalctl -u <your-service-name>.service -f```
