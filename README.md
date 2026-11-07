# OpenRelik

Every component of OpenRelik in one repository. Each was imported from its own
repository with its full history; the old repositories are archived.

| Directory            | What                                  | From                  |
| -------------------- | ------------------------------------- | --------------------- |
| server               | API, mediator, metrics, migrations    | openrelik-server      |
| web/sunstone         | web UI, codename sunstone (see web/)  | openrelik-ui          |
| workers              | task workers                          | openrelik-workers     |
| mcp                  | MCP server                            | openrelik-mcp-server  |
| libs/common          | shared Python library                 | openrelik-common      |
| libs/ai-common       | shared Python library (AI)            | openrelik-ai-common   |
| libs/python-client   | Python API client                     | openrelik-api-client  |
| libs/worker-common   | shared library for workers            | openrelik-workers     |
| deploy               | production deployment                 | openrelik-deploy      |

## License

Apache License 2.0, see [LICENSE](LICENSE).
