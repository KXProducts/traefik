# Redis Provider

Traefik can be configured to use Redis as a provider.

```toml
################################################################
# Redis Provider
################################################################

# Enable Redis Provider.
[redis]

# Redis server endpoint.
#
# Required
# Default: "127.0.0.1:6379"
#
endpoint = "127.0.0.1:6379"

# Enable watch Redis changes.
#
# Optional
# Default: true
#
watch = true

# Prefix used for KV store.
#
# Optional
# Default: "traefik"
#
prefix = "traefik"

# Override default configuration template.
# For advanced users :)
#
# Optional
#
# filename = "redis.tmpl"

# Use Redis user/pass authentication.
#
# Optional
#
# username = foo
# password = bar

# Enable Redis TLS connection.
#
# Optional
#
#    [redis.tls]
#    ca = "/etc/ssl/ca.crt"
#    cert = "/etc/ssl/redis.crt"
#    key = "/etc/ssl/redis.key"
#    insecureSkipVerify = true
```

To enable constraints see [provider-specific constraints section](/configuration/commons/#provider-specific).

Please refer to the [Key Value storage structure](/user-guide/kv-config/#key-value-storage-structure) section to get documentation on Traefik KV structure.
