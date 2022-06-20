## 🪖 Conceitos e comandos

#### 1. Repositório

- Armazenamento virtual do projeto
- Cada projeto deve ter seu próprio repo
  - esse é o modelo ideal, é possível manter vários projetos no mesmo repositório usando o modelo monorepo
- Permite registrar e visualizar as versões do código
- Possui uma subpasta `.git`

  - essa pasta mantém os registros do repo localmente

  ![Exemplo de projeto com o git](./../assets/images/git-commands-01.png)
  _O projeto git possui uma pasta oculta `.git`, que mantem o histórico._

##### 1.1. Iniciando o Git

- `git init`[🔗](https://git-scm.com/docs/git-init/pt_BR)
  - inicializa um repositório “zerado” no diretório selecionado
  - usado quando se inicia a pasta não é um repo do git

<br/>

- `git clone`[🔗](https://git-scm.com/docs/git-clone/pt_BR)
  - copia o conteúdo do repositório no diretório e cria as associações com o repositório original
  - usado para trabalhar em projetos já iniciados
  - _veremos o funcionamento nas próximas sessões_
