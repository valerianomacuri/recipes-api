# Rescipes APIRestful

## Git alias

Para mostrar el `status`:

```console
git config --global alias.s "status --short"
```

Para mostrar los `logs`:

```console
git config --global alias.lg "log --graph --abbrev-commit --decorate --format=format:'%C(bold blue)%h%C(reset) - %C(bold green)(%ar)%C(reset) %C(white)%s%C(reset) %C(dim white)- %an%C(reset)%C(bold yellow)%d%C(reset)' --all"
```

Gist de los alias [click aquí](https://gist.github.com/Klerith/0acf18bbece7923bcac55edb71b03c2b).

## Instalar go-swagger

[https://goswagger.io/install.html](https://goswagger.io/install.html)

En caso de instalar desde el código fuente, crear un alias en el archivo `.zshrc`:

```console
alias swagger='~/go/bin/swagger'
```

### Generar `swagger.json`

```console
swagger generate spec -o ./swagger.json --scan-models
```

### Abrir el Swagger UI con la configuración del `swagger.json`

```console
swagger serve -F swagger ./swagger.json
```