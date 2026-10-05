# Container Observability

## Application Logs

The following log line shows the 404 error generated when the requested page did not exist:

```text
172.17.0.1 - - [05/Oct/2026:15:49:22 +0000] "GET /hidden-admin-page HTTP/1.1" 404 153 "-" "curl/8.5.0" "-"
```

Application logs are important because they show the requests and errors happening inside the application. They help Cloud Operations Engineers identify problems and troubleshoot issues based on actual events instead of guessing.

