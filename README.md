# Vector Role

Ansible role for installing and configuring Vector.

## Requirements

- Ubuntu 20.04/22.04, Debian 11/12
- Ansible 2.9+

## Role Variables

| Variable | Description | Default |
|----------|-------------|---------|
| `vector_version` | Vector version | `0.31.0` |
| `vector_clickhouse_host` | ClickHouse host | `127.0.0.1` |
| `vector_clickhouse_port` | ClickHouse port | `8123` |
| `vector_clickhouse_database` | Database name | `logs` |
| `vector_clickhouse_table` | Table name | `nginx_logs` |

## Example

```yaml
- hosts: servers
  roles:
    - vector-role
