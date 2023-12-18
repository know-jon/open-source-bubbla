För att komma igång med [rill](https://www.rilldata.com/) ställ dig i root katalogen för denna projektet

Kör kommandot i ett skal eller kommandoterminal

```shell
curl -s https://cdn.rilldata.com/install.sh | bash
rill start my-rill-project
```

Observera att detta laddar ner och installerar saker från internet.

För att använda en existerande duckdb från till exempel den vi skapade i work så kan du inkludera den genom att skriva

```shell
rill start --db work/duckdb.db my-rill-project
```