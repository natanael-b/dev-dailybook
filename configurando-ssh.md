Para utilizar o `dev-dailybook` é necessário configurar uma chave SSH para fazer issso:

# Chave pública
- No navegador, acesse [https://github.com/settings/ssh/new](https://github.com/settings/ssh/new)
- Dê um nome para a chave
- Abra um terminal e digite o comando e dê Enter:

```bash
 echo "chave-dev-dailybook" | ssh-keygen -t ed25519 -C "your_email@example.com"
```
- Cole o conteúdo do arquivo `chave-dev-dailybook.pub`
- Clique em `Add SSH key`

# Chave privada

- Abra o repositório do GitHub Pages
- Clique:
  - `Settings`
    - `Secrets and variables`
      - `Actions`
        - `New repository secret`
- Em `Name` coloque `SSH_PRIVATE`
- Em `Secret` cole o conteúdo do arquivo `chave-dev-dailybook`

# Finalização

Apague os arquivos `chave-dev-dailybook.pub` e `chave-dev-dailybook`, siga o [`README.md`](README.md)
