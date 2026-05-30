# Setup MySQL environment

Configure the MySQL service container.

## Example Usage

```
  execute-test:
    runs-on: ubuntu-latest
    services:
      mysql:
        image: mariadb
        env: { "MARIADB_ALLOW_EMPTY_ROOT_PASSWORD": "1" }
        ports: [3306:3306]
    steps:
      - uses: infrabits/ci-setup-mysql@main
```
