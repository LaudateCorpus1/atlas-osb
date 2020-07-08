# MongoDB Atlas Service Broker

ACTIVE WORKING DETACHED FORK of [https://github.com/mongodb/mongodb-atlas-service-broker](https://github.com/mongodb/mongodb-atlas-service-broker)

Use the Atlas Service Broker to connect to [MongoDB Atlas](https://www.mongodb.com/cloud/atlas) from any platform which supports the [Open Service Broker API](https://www.openservicebrokerapi.org/), such as [Kubernetes](https://kubernetes.io/) and [Pivotal Cloud Foundry](https://pivotal.io/open-service-broker).

- Provision managed MongoDB clusters on Atlas directly from your platform of choice. Includes support for all cluster configuration settings and cloud providers available on Atlas.
- Manage and scale clusters without leaving your platform.
- Create bindings to allow your applications access to clusters.

## Documentation

For instructions on how to install and use the MongoDB Atlas Service Broker please refer to the [documentation](https://docs.mongodb.com/atlas-open-service-broker).

## Configuration

Configuration is handled with environment variables. Logs are written to
`stderr` and each line is in a structured JSON format.

| Variable | Default | Description |
| -------- | ------- | ----------- |
| ATLAS_BASE_URL | `https://cloud.mongodb.com` | Base URL used for Atlas API connections |
| BROKER_HOST | `127.0.0.1` | Address which the broker server listens on |
| BROKER_PORT | `4000` | Port which the broker server listens on |
| BROKER_LOG_LEVEL | `INFO` | Accepted values: `DEBUG`, `INFO`, `WARN`, `ERROR` |
| BROKER_TLS_CERT_FILE | | Path to a certificate file to use for TLS. Leave empty to disable TLS. |
| BROKER_TLS_KEY_FILE | | Path to private key file to use for TLS. Leave empty to disable TLS. |
| PROVIDERS_WHITELIST_FILE | | Path to a JSON file containing limitations for providers and their plans. |

## License

See [LICENSE](LICENSE). Licenses for all third-party dependencies are included in [notices](notices).

## Development

Information regarding development, testing, and releasing can be found in the [development documentation](dev).
