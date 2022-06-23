## 4. Tags

- Um snapshot de um branch que não se modifica
- Usadas para controle de releases e versões
- É possível criar branches a partir de tags para correções

> Normalmente as pessoas usam essa funcionalidade para marcar pontos onde foram feitas releases (v1.0 e assim por diante)
> [_Pro Git book, escrito por Scott Chacon e Ben Straub_](https://git-scm.com/book/pt-br/v2/Fundamentos-de-Git-Criando-Tags)

### 3.1. Criando e listando os branches

- `git tag`[🔗](https://git-scm.com/docs/git-tag/pt_BR)

  - lista, cria e deleta branches

### 4.1. Criando e listando tags

#### 👨🏽‍💻 Mão na massa

```bash
# lista as tags criadas
git tag

# cria a tag
git tag v0.0.1

# cria a tag com uma mensagem de log
git tag v0.0.1 -m "new release version"
```

### 4.2. Criando um branch a partir de uma tag

#### 👩🏼‍💻 Mão na massa

```bash
# cria e o muda o contexto para o branch
# "new-branch" a partir da tag "v0.0.1"
git checkout -b new-branch v0.0.1
```

---

[🏠 Voltar para o início](./../README.md)

[⬅️ Branches](./git-commands-03.md) | [Merging ➡️](./git-commands-05.md)
