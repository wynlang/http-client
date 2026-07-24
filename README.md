# http-client

An HTTP client is **built in** to Wyn - no package needed. Use the `Http`
module directly:

```wyn
var body = Http.get("https://api.example.com/users")
var resp = Http.post("https://api.example.com/users", "{\"name\":\"Alice\"}")

Http.set_header("Authorization", "Bearer your-token")
Http.set_header("Content-Type", "application/json")
var me = Http.get("https://api.example.com/me")
Http.clear_headers()
```

This repository previously shipped a thin `HttpClient_*` wrapper that only
forwarded to those built-ins, so it has been emptied to this note.
