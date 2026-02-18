# http-client — Official Wyn Package

HTTP client with JSON, headers, and auth. Pure Wyn, wraps built-in Http module.

## Install

```bash
wyn pkg install github.com/wynlang/http-client
```

## Usage

```wyn
// Simple GET
var body = HttpClient_get("https://api.example.com/users")

// POST JSON
var resp = HttpClient_post_json("https://api.example.com/users", "{\"name\":\"Alice\"}")

// With auth
var data = HttpClient_get_auth("https://api.example.com/me", "your-token")
```

## Test

```bash
wyn run tests/test_http_client.wyn
```
