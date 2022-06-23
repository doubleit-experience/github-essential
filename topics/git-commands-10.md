## 9. Push & Pull

Informa seu git local que ele deve obter as informações de metadados mais recentes do repositório remote (embora ainda não faça a transferência dos dados – é como verificar para ver se há mudanças disponíveis).

---

### 8.1. Sincronizando metadados do remote

- `git fetch`[🔗](https://git-scm.com/docs/git-fetch/pt_BR)
  - baixa objetos e referências de outros repos (remotes)
  - sincroniza metadados dos branches, tags, commits, etc, mas não os arquivos em si

#### 👨🏻‍💻 Mão na massa

```bash
# baixa as referências do remote ORIGIN
git fetch origin

# baixa as referências do remote ORIGIN, apenas branch-01
git fetch origin branch-01

# baixa todas as referências para todos
# os remotes e todos os branches
git fetch --all
```

Importante notar que até aqui apenas criamos a conexão do repo local com outro repo (o remote), e sincronizamos os metadados, ainda não "baixamos os arquivos" localmente. É o que veremos nos próximos comandos.

---

[🏠 Voltar para o início](./../README.md)

[⬅️ Remotes](./git-commands-07.md) | [Push ➡️](./git-commands-09.md)
