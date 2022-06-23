## 🔀 Workflows

São formas de trabalhar e padronizar o uso dos branches dentro de um projeto para proteger e simplificar o “código entregável”

### Características do git que permitem flexibilidade

- 🔛 Distribuído
  - cada usuário possui todo o repo localmente
- 🌳 Ramificações simplificadas
  - é muito fácil criar e gerenciar branches
- 🤝 Contribuições
  - é muito simples criar associações com repositórios (remotes) para sincronizar informações

Em contraste com os “Centralized Version Control Systems” (CVCSs), o git permite que você seja muito mais **flexível na forma dos desenvolvedores contribuírem com os projetos**.

Abaixo seguem alguns modelos de workflow usados com o Git

#### Centralized Workflow

- simula um CVCS (sistemas centralizados)
- fluxo muito comum na maior parte das equipes
- o Git não permite que você faça um push se não tiver com a última versão sincronizada
- esse fluxo garante que todos só possam fazer alterações depois de sincronizar com o repo central

![Centralized Workflow](./../assets/images/git-workflows-01.png)

#### Integration-Manager Workflow

- apenas uma pessoa pode commitar em um repo "abençoado"
- os devs clonam do repo "abençoado" e sincronizam dali
- após fazer as mudanças, os devs fazem um pull request (para aprovação do gerente de integração) para incluir no repo "abençoado"
- modelo muito usado em open source

![Integration-Manager Workflow](./../assets/images/git-workflows-02.png)

#### Dictator and Lieutenants Workflow

![Dictator and Lieutenants Workflow](./../assets/images/git-workflows-03.png)

---

[🏠 Voltar para o início](./../README.md)
