## 9. Push & Pull

Sincronizam de fato os arquivos num determinado remote, enviando (push) ou recebendo (pull) as atualizações.

---

### 9.1. Recebendo atualizações

- `git pull`[🔗](https://git-scm.com/docs/git-pull/pt_BR)
  - faz um fetch e um merge com o branch do remote
  - atualiza os objetos locais
  - sincroniza os arquivos (merge) e pode gerar conflitos locais

#### 👩🏻‍💻 Mão na massa

```bash
# faz um fetch e um merge das atualizações do remote
# com o local, apenas para o branch corrente
git pull origin
```

### 9.2. Enviando atualizações

- `git push`[🔗](https://git-scm.com/docs/git-push/pt_BR)
  - atualiza o remote com as referências e objetos locais

#### 👨🏼‍💻 Mão na massa

```bash
# após realizar os commits, você pode usar o push
# para enviar suas alterações no repo local para o remote

# envia todas as referências e objetos (arquivos)
# de MAIN para o remote ORIGIN
git push origin main

# envia todos os branches
git push origin --all

# envia todas as tags
git push origin --tags
```

---

[🏠 Voltar para o início](./../README.md)

[⬅️ Fetch](./git-commands-08.md) | [Considerações finais... ➡️](./git-commands-10.md)
