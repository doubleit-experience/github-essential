## 📗 Entenda o funcionamento

Além de entender como funcionam os comandos do git, é importante compreender alguns conceitos teóricos fundamentais. Dessa forma, será possível usar essa ferramenta de forma muito mais eficiente.

<!-- https://www.lumis.com.br/a-lumis/blog/git-conceitos-basicos.htm -->

#### 1. Snapshots, não diferenças

- Em cada commit, todo o estado do projeto é salvo
- Se o arquivo não foi modificado, o Git salva um link para a última alteração do

![Linha do tempo de checkins](./../assets/images/git-concepts-02.png)
_Armazenando dados como um estado do conjunto de arquivos do projeto ao longo do tempo._

> Isso faz com que o Git seja mais como um mini sistema de arquivos com algumas ferramentas incrivelmente poderosas, ao invés de simplesmente um VCS.
> [_Pro Git book, escrito por Scott Chacon e Ben Straub_](https://git-scm.com/book/pt-br/v2/Come%C3%A7ando-O-B%C3%A1sico-do-Git)

#### 2. Quase toda operação é local

- A maioria das operações acontece na sub-pasta `.git`
- Todos os registros do git ficam armazenados nessa pasta
- Isso faz as operações do git serem praticamente instantâneas

- O clone inicial é mais lento, pois faz uma cópia completa do repo
  - Quanto mais commits, branches, tags e histórico o repo tiver, maior será o conteúdo em .git

> Se você estiver acostumado com um CVCS onde a maioria das operações têm aquela demora causada pela latência da rede, este aspecto do Git vai fazer você pensar que os deuses da velocidade abençoaram o Git com poderes extraterrestres. Como você tem toda a história do projeto ali mesmo em seu disco local, a maioria das operações parecem quase instantâneas.
> [_Pro Git book, escrito por Scott Chacon e Ben Straub_](https://git-scm.com/book/pt-br/v2/Come%C3%A7ando-O-B%C3%A1sico-do-Git)

#### 3. Git tem integridade

- Todas as operações passam por “checksum” antes de ser armazenadas
- Cada operação é associada ao código obtido
- Usa [SHA-1 hash](https://en.wikipedia.org/wiki/SHA-1)
- O git armazena tudo em base não pelo nome do arquivo, mas pelo hash do seu conteúdo. Ex: `24b9da6552252987aa493b52f8696cd6d3b00373`

> Tudo no Git passa por uma soma de verificações (checksum) antes de ser armazenado e é referenciado por esse checksum. Isto significa que é impossível mudar o conteúdo de qualquer arquivo ou pasta sem que Git saiba.
> [_Pro Git book, escrito por Scott Chacon e Ben Straub_](https://git-scm.com/book/pt-br/v2/Come%C3%A7ando-O-B%C3%A1sico-do-Git)

#### 4. Git geralmente apenas adiciona dados

- Praticamente todas as ações no git adicionam informações à base local
- Isso garante que você possa reverter praticamente qualquer alteração (desde que commitadas)
- Isso também faz com que a base de histórico em .git cresça consideravelmente

> Isso faz com que o uso do Git seja somente alegria, porque sabemos que podemos experimentar sem o perigo de estragar algo.
> [_Pro Git book, escrito por Scott Chacon e Ben Straub_](https://git-scm.com/book/pt-br/v2/Come%C3%A7ando-O-B%C3%A1sico-do-Git)

#### 5. Os três estados

- O fluxo básico de trabalho no Git é o seguinte:

  - **MODIFIED**: Você modifica os arquivos na “working tree”
  - **STAGED**: Você envia os arquivos selecionados para “stage”
  - **COMMITED**: Você faz um commit, que envia os arquivos como estão de “stage” para .git (adiciona um snapshot do repo)

    <br/>

![Diretório de trabalho, área de preparo, e o diretório Git](./../assets/images/git-concepts-01.png)

> Esta é a principal coisa a lembrar sobre Git se você quiser que o resto do seu processo de aprendizagem ocorra sem problemas. O Git tem três estados principais que seus arquivos podem estar: committed, modificado (modified) e preparado (staged).
> [_Pro Git book, escrito por Scott Chacon e Ben Straub_](https://git-scm.com/book/pt-br/v2/Come%C3%A7ando-O-B%C3%A1sico-do-Git)
