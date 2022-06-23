## 3. Branches

- Cópias (independentes) da “linha principal” do código do repo
- main/master é o branch inicial que representa a linha principal de desenvolvimento
  - atualmente, para novos repos, o nome "master" não é mais usado por questões relacionadas ao termo "master - slave" que remete ao período de escravidão
- Abstração do processo de “edit/stage/commit” - novos registros de histórico
- Os nomes podem ser definidos, não há nomes reservados
- No git, a manipulação de branches é simples e performática

> A forma como o Git cria branches é incrivelmente leve, tornando as operações de ramificação quase instantâneas, alternando entre os branches geralmente com a mesma rapidez. Ao contrário de muitos outros sistemas, o Git incentiva fluxos de trabalho que se ramificam e se fundem com frequência, até mesmo várias vezes ao dia. **Compreender e dominar esse recurso oferece uma ferramenta poderosa e única e pode mudar totalmente a maneira como você desenvolve**.
> [_Pro Git book, escrito por Scott Chacon e Ben Straub_](https://git-scm.com/book/pt-br/v2/Branches-no-Git-Branches-em-poucas-palavras)

### Características de uso de branches

A facilidade em gerenciar branches pelo Git permite algumas características que influenciam a produtividade e a forma de trabalho das equipes.

- 🔀 **Mudança de contexto sem atritos**
  - é muito fácil mudar de branches pelo Git e desenvolver em paralelo
    <br/>
- ✳️ **Linhas de código baseadas em função**
  - é possível criar branches com funções diferentes (um para produção, outro para testes, etc)
    <br/>
- ⚛️ **Fluxo baseado em funcionalidades**
  - é possível criar branches específicos para criar funcionalidades diferentes
    <br/>
- 🚮 **Experimentação descartável**
  - criar branches e testar mudanças é muito simples, em caso de erros ou descarte da ideia, basta remover o branch

### 3.1. Criando e listando os branches

- `git branch`[🔗](https://git-scm.com/docs/git-branch/pt_BR)

  - lista, cria e deleta branches
    <br/>

- `git checkout`[🔗](https://git-scm.com/docs/git-checkout/pt_BR)
  - troca de branches
  - o Git tem um "ponteiro" que indica um dos branches para ser o "corrente"

#### 👩🏼‍💻 Mão na massa

```bash
git branch # lista todos os branches criados (localmente)
# e destaca o branch corrente

# cria o branch
git branch novo-branch

# outra forma de criar um branch, mas esse comando, além da
# criação, já troca para o branch criado
git checkout -b novo-branch

# retorna para o branch main
git checkout main
```

### 3.2. Renomeando e removendo branches

```bash
# renomeia o branch para branch-01
git branch -m branch-01

# remove o branch - importante commitar e dar "push" em tudo antes
git branch -d branch-01
```

---

[🏠 Voltar para o início](./../README.md)

[⬅️ Commit](./git-commands-02.md) | [Tags ➡️](./git-commands-04.md)
