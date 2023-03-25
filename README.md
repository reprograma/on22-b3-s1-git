<h1 align="center">
  <img src="assets/reprograma-fundos-claros.png" alt="logo reprograma" width="500">
</h1>

# Conceitos básicos, Git, Github e versionamento de código

Turma Online 22 - B3  | Back-end | Semana 1 | 2023 | Professora [Sky Alarcón ☁](https://www.instagram.com/_skydoceu/?hl=pt-br)

### Instruções
Antes de começar, vamos organizar nosso setup.
* Fork esse repositório 
* Clone o fork na sua máquina (Para isso basta abrir o seu terminal e digitar `git clone url-do-seu-repositorio-forkado`)
* Entre na pasta do seu repositório (Para isso basta abrir o seu terminal e digitar `cd nome-do-seu-repositorio-forkado`)
* Não tenha vergonha, a única dúvida ruim é a dúvida que não foi sanada!
* Para fazer perguntas, basta levantar a mão que a professora ou monitora vão te chamar
* Beba água e respire fundo. Vamos aos poucos trilhar essa jornada
* **Seja curiosa!** Experimente, teste, mude o código, invente e se permita explorar!

### Resumo
O que veremos na aula de hoje?
* [Conceitos básicos](#Conceitos-básicos)
* [Terminal e versionamento de código](#Terminal-e-versionamento-de-código)
* [Git & GitHub](#Git-&-GitHub)

## Conteúdo
### Conceitos básicos
1. [Programação](#programa%C3%A7%C3%A3o)
2. [Back, Front, Fullstack e Mobile](#back-front-fullstack-e-mobile)
3. [Client-side e Server-side](#client-side-e-server-side)
4. [Algoritmo e Pseudocódigo](#algoritmo-e-pseudoc%C3%B3digo)


### Terminal e versionamento de código
1. [Terminal](#terminal)
2. [Versionamento de código](#versionamento-de-c%C3%B3digo)

### Git & GitHub
1. [Git](#git--github-1)
  * [Gitflow](#git)
  * [Comandos](#comandos)

2. [GitHub](#github)
  * [Comandos](#comandos-1)
  * [Commits semânticos](#commits-sem%C3%A2nticos)
  * [Markdown](#markdown)

### [Exercícios](#exerc%C3%ADcios-1)

### [Links úteis](#links-%C3%BAteis-1)

# Conceitos básicos 

## Programação


 ### **O que é programação?**

  ```
 Programação é o processo de escrita, teste e manutenção de um programa 
 de computador. O programa é escrito em uma linguagem de programação, 
 embora seja possível, com alguma dificuldade, o escrever diretamente 
 em linguagem de máquina. Diferentes partes de um programa podem ser 
 escritas em diferentes linguagens.
  ```

  Para começar, vamos diferenciar duas coisas: **hardware** e **software**.
  > *Hardware*: São os elementos **FÍSICOS** do computador, como o `monitor`, `teclado`, `processador`, etc
  
  > *Software*: É o que fala para as peças físicas **O QUE FAZER**, como os `editores de foto`, `sistemas operacionais`, etc 

  Muito importante lembrar que, apesar de não parecer, o computador é apenas uma pedra que damos choquinhos e faz contas muito rápido por caisa disso. Todo e qualquer processo no computador foi criado um conjunto de regras lógicas e sequenciadas para que, ao executar entreguem o resultado desejado de forma que a nova informação adquirida seja utilizável pela usuária.

  Pelo fato de programar ser um processo EXTREMAMENTE LITERAL, precisamos, não só aprender seus comandos, mas também como desestruturar nossos problemas em problemas menores que sejam realizáveis por ideias/comandos simples que podemos transcrever como um código para o computador executar.

  Agora surge a pergunta, onde a gente entra nisso tudo?

  Desenvolvedoras (ou `devs`, como abreviamos) desenvolvem softwares para criar programas que resolvam problemas. Lembrando que um dos maiores motivos desses problemas é a velocidade em que ele processa nossos dados e entrega resultados, por isso inventaram um conceito de programação: **KISS**.

  * **K**eep
  * **I**t
  * **S**tupidly
  * **S**imple

  Traduzindo: Mantenha aquilo **estupidamente** simples

  Para isso, é muito importante estudarmos `lógica de programação`, `código limpo (clean code)` e usar outras formas de deixar nosso código fácil de ler por outras `devs` para que a manutenção (pois o código *VAI* quebrar e é importante sabermos lidar), aprimoramento do código e implementação de novas linhas para novos processos seja possível.


  ## Back, Front, Fullstack e Mobile

  Em qualquer programa que use teremos, geralmente, dois setores em que `devs` fazem parte: Back-end e Front-end.

  > Back-end: Tudo que está por trás das telas, processos que usuárias não terá acesso direito e não vai interagir *diretamente*

  > Front-end: Corresponde a tudo que o usuário ve e/ou interage com, como menus, imagens, etc.

  Falta explicar o `Fullstack` e `Mobile`. Esses dois termos são mais simples do que parecem.
  
  `Fullstack` é a `dev` que trabalha com **AMBAS** as áreas, Back *E* Front-end, portanto essa pessoa fará as funções que uma usuária não teria acessa (processamento de dados) e também as telas e menus dos programas.

  E por último, `Mobile` é a `dev` que criará **aplicativos** (também chamados de *apps*). Hoje em dia temos diversos sistemas operacionais (também chamaods de *OS*), como Android e iOS sendo os mais conhecidos e amplamente usados no mercado.


  ## Client-side e Server-side

  O cliente é sempre quem inicia as comunicações com o servidor. O cliente mais comum é um `navegador`. Ao acessar um site pelo navegador, uma requisição é feita, pela internet, para o servidor onde está o site. O papel desse servidor é devolver uma resposta para o cliente (nesse caso, o navegador). Normalmente, um servidor **NÃO** envia nenhum dado para cliente sem que haja um requisição antes.

  O servidor é um local que vai receber as requisições do cliente, processar parte dos dados e devolver as informações necessárias para que o cliente continue suas opreçãoes.

  Quando falamos de desenvolvimento web, um modelo muito usado é o *cliente-servidor*, pois o servidor é um local seguro e confiável e contido em ambiente controlado em que é possível armazenar os dados de usuárias e os processar. Esses ambientes controlados garantem o funcionamento 24/7 das máquinas que rodam o servidor para que não deixem de receber nenhuma requisição ou deixar de enviar alguma resposta.

  Um único servidor é capaz de responder diversos clientes simultaneamente para que qualquer usuária tenha suas informações no instante que precisarem.


  ## Algoritmo e Pseudocódigo

  ### **Algoritmo**

  Antes de escrevermos nosso código, precisamos saber o que o programa deverá fazer e, com isso, quais serão os passos tomados para executar a tarefa definida. Para isso, criamos um conjunto de regras chamado **algoritmo**. O `algoritmo` não é, por si só, o programa. Em sua definição, ele é um grupo de comandos executáveis pelo nosso computador que, de acordo com a sequência e condições exigidas, calculará nosso resultado esperado.

  Comandos como "enquanto [algo], faça [algo]" ou condicionais "se [algo], então [algo]"

  ### **Pseudocódigo**

  Nosso `algoritmo` pode ser representado de diversas formas distintas. Uma delas é como um **pseudocódigo**, que nada mais é que uma série de instruções que nós, humanas, conseguimos interpretamos, porém precisaríamos codar as linhas para que um computador nos entendesse. Um exemplo muito simples são receitas para preparo de comida. Você segue as instruções e, ao fazer todas as ações de maneira correta, chega no resultado esperado que pode ser refeição completa, uma sobremesa, etc.

  Outra forma de apresentar esse algoritmo é por um fluxograma, como por exemplo:

  <img src="assets/fluxograma.png">


# Terminal e versionamento de código

  ## Terminal
  Lembra daquela tela preta que hackers dos filmes sempre tem aberta no computador pra invadir o sistema do FBI ou da NASA? Aquilo é o terminal. No começo, o terminal pode acabar assustando um pouco, ele tem pouca informação, precisa de comandos específicos para funcionar, mas não se deixe intimidar, é mais tranquilo do que parece (não disse que é fácil, mas não é difícil).

  O terminal age como a tela do nosso computador, mas sem todos os ícones, apenas texto, então pode ser um pouco menos intuitivo em um primeiro momento.

  Existem vários comandos distintos para fazer as mais diversas funções dentro do terminal. Na teoria, a quantidade de comandos possíveis são *infinitos*, pois outros programas podem adicionar novos comandos para executar tarefas específicas.

  ## Versionamento de código

  Para controlar qual versão será disponibilizada para o público, usamos uma técnica chamada `versionamento de código`. Ela consiste em atualizar aos poucos nosso programa para que todas as funcionalidades sejam testas das mais diversas formas para que tenhamos certeza que nossa usuária não encontrará `bugs` durante sua utilização.

  Essa técnica é um *ótima prática* para equipes de `devs`, pois, se a equipe inteira não trabalhar na mesma função, alguém não saberá o que aconteceu e, ao atualizar o sistema, pode haver falhas que antes não existiam e será mais difícil identificá-las.

  Para `devs` solo também é uma prática interessante a ser feita para que, ao desenvolver ou atualizar o código, é possível manter um controle do que estava funcionando e o que precisava ser feito para que, no final do dia, qualquer pessoa q acesse seu serviço consiga usar sem encontrar muitos problemas.

# Git & GitHub
  ## Git
  `Git` é uma ferramenta de controle de versão *`open source`* (ou seja, de código aberto. Qualquer pessoa na internet pode ver as linhas de comando e estudar como o código executa cada uma de suas funcionalidades). O `Git` tem seu maior foco em velocidade e integridade de seus dados. Com esses dois objetivos em mente, `Git` nos permite que duas (ou mais) pessoas, **ao mesmo tempo**, trabalhem **no mesmo código** sem que nenhuma parte do desenvolvimento seja perdido por uma pessoa ter salvado seu progresso em cima do da outra.

  Uma parte importante dessa ferramenta é a possibilidade de ver o histórico de modificações e, se algo der errado, voltar para versões anteriores.

  Para fazer o download, basta clicar na imagem abaixo:

  <h1 align="center">
  <a href="https://git-scm.com/downloads"><img src="assets/Git-Icon-1788C.png"></a>
  </h1>

  ### **Gitflow**
  `Gitflow` é uma forma alternativa de fazer seu versionamento de código. Ele terá uma ramificação primária. Outras ramificações são criadas para que o código seja aprimorado com novas funcionalidades, otimizações ou outras coisas. Após verificar que o novo desenvolvimento está funcionando sem problemas, é feito o *`merge`* (traduzindo literalmente para `fusão`) do código novo com as linhas modificadas ao código já existente.

  Cada recurso novo criará a própria *`branch`* (ramificação), implementará o novo código nela e, ao final de tudo, pode ser enviada para a `branch` principal para que ocorra o `merge`.

  <h1 align="center">
  <img src="assets/gitflow.jpg">
  </h1>

  Na imagem podemos observar como é feito o desenvolvimento do programa. Existe a `branch` principal (em azul claro) e `branches` secundárias. Toda vez que é lançada uma nova versão de um programa, significa que houve um `merge` de uma ou mais `branches` secundárias à `branch` principal.

  Notamos também a possibilidade de ramificar `branches` secundárias se necessário.

  ### **Comandos**
  Vamos aprender alguns comandos do `Git`

  Comando                                              | Descrição
  -----------------------------------------------------|-------------------------------------------------------
  git config user.name "Username da Reprogramer"       | configura o seu username no github
  git config user.email "emailDaReprogramer@gmail.com" | configura o seu email utilizado para logar no github
  git config --list                                    |  mostra todas as propriedades de configuração do Git
  ls                                                   | listar (ele traz uma lista de tudo o que está naquela pasta - documentos, outras pastas, etc)
  mkdir nome-da-pasta                                  | cria uma pasta
  touch nome-do-arquivo                                | cria um arquivo
  cd                                                   | usado para se locomover entre as pastas
  cd ~                                                 | volta para a pasta raiz
  cd ..                                                | volta uma pasta
  pwd                                                  | traz o caminho onde você está (em que pasta e onde essa pasta fica)
  rm arquivo                                           | remove, deleta um arquivo. (**cuidado! Ele não solicita confirmação**)
  rm -f ou rm --recursive pasta                        | deleta uma pasta (**cuidado! Ele não solicita confirmação**)
  whoami                                               | "quem sou eu?" identifica o usuário que está mexendo no sistema
  git init                                             | inicializa o git no repositório local


  ## Github
  [Github](https://github.com/) é um site que permite a hospedagem de repositórios (projetos) utilizando o `Git`. Ouras pessoas podem ver seus projetos, o código deles, baixar, estudar e desenvolver junto (esse último demanda permissões da usuária dona do projeto). Assim como outras pessoas, você pode fazer o mesmo com o código de outras pessoas. O [Github](https://github.com/) funciona como uma espécie de rede social muito utilizada por desenvolvedores na qual você tem a chance de compartilhar seus projetos pessoais e particulares, alpem de contribuir com projetos de outras pessoas ou empresas do mundo todo.

  O [Github](https://github.com/) é uma ferramente mais visual que o `Git`, porém contém diversas funcionalidades extremamente similares para fazer o versionamento de código.

  Nosso resumo da ópera: Você trabalha da sua máquina, salva a versão do código no [Github](https://github.com/) e pode contribuir em projetos de outras pessoas, além de baixar e estudar o código delas para seu computador.

  Agora uma pergunta importante é: **Por que o [Github](https://github.com/) é tão importante?**

  1. Portifólio - O [Github](https://github.com/) é um local seguro para armazenar e mostrar seus projetos. Não é incomum as empresas pedirem seu [Github](https://github.com/) antes de uma entrevista de emprego.

  2. Organização - Permite que todoas as pessoas trabalhem no mesmo projeto (seja um projeto pessoal, da empresa ou até mesmo `open source`)

  Agora chegou a hora de criarmos a nossa conta! Clique na imagem para acessar o [Github](https://github.com/)

  <h1 align="center">
  <a href="https://github.com/"><img src="assets/github.png"></a>
  <h1>

  ### **Comandos**
  Vamos ver alguns comandos para utilizar o [Github](https://github.com/) a partir do `Git`

  Comando                         | Descrição
--------------------------------|-------------------------------------------------------
git add nome-do-arquivo         | adiciona um arquivo modificado ao stagging (área temporária) 
git add .                       | adiciona todos os arquivos modificados ao stagging (área temporária) 
git status                      | mostra os status dos arquivos modificados
git commit -m "mensagem"        | cria um commit
git pull                        | puxa as atualizações mais recente (remoto -> local)
git push                        | envia as atualizações mais recentes (local -> remoto)
git remote add origin nome-da-branch   | faz um link entre seu repositório local com o remoto 
git checkout -- nome-arquivo    | descarta as alterações locais do arquivo informado
git checkout -b nome-da-branch  | cria uma branch a partir da atual
git checkout nome-da-branch     | troca de branch
git merge nome-da-branch        | mescla a branch passada no parâmetro com a atual
git remote -v                   | mostra as URLs para onde o git está apontando
git log                         | mostra o histórico de commits, com data, hora, mensagem e autora (caso fique presa nessa lista, aperte "q" para sair)
git branch                      | lista todas as branchs locais
git diff                        | mostra no terminal a diferença entre os arquivos editados localmente

  **Alguns conceitos básicos que vamos usar a partir de hoje no GitHub**

  * **Repositório**: espaço digital aonde o seu projeto vai ser salvo. No seu computador ele é a pasta aonde o seu projeto está salvo.

  * **Commit**: controle de versão (histórico) daquele arquivo e cria uma etiqueta para facilitar o entendimento do que foi salvo naquele momento.

  * **Pull**: serve para se comunicar entre a sua máquina e o repositório remoto. Esse comando faz uma cópia do repositório remoto e baixa ele para a sua máquina.

  * **Push**: serve para se comunicar entre a sua máquina e o repositório remoto. Esse comando faz uma cópia do repositório local e envia ele para o repositório remoto.

  * **Clone**: faz exatamente o que ele sugere: uma cópia exata do arquivo, que você vai baixar do repositório remoto para a sua máquina.

  * **Branch**: permite que cada usuário tenha o seu "galho" dentro de um projeto de maneira independente. Ela é uma parte muito útil no desenvolvimento em um projeto coletivo.

  * **Merge**: unifica diferentes branches

  * **Fork**: cria uma cópia de um projeto para o seu GitHub

  * **Pull Request(PR)**: solicitação de dar merge da sua branch em um projeto de outra pessoa

  ### **Commits semânticos**

  **Commit semântico** (ou *`conventional commit`*) é a prática de *PADRONIZAÇÃO* das mensagens de `commits` dentro de um projeto de desenvolvimento de software.

  Uilizando regras simples e claras, que apesar de inroduzirem uma pequena carga a mais de trabalho, vai contribuir para que seja reduziado o tempo gasto em compreender como e por que algo foi feio em uma alteteração ou correção posterior do código.

  Na rotina de `dev` solo, não parece que existem muitos benefícios, porém, com a introdução de um time que trabalha simultaneamente no mesmo projeto em um mesmo repositório centralizado, há um aumento da agilidade de compreensão do que seus pares desenvolveram e corrigiram no código já existente.

  Algumas vantagens dos `commits semânticos` são:
   - Possibilitar a adoção de processos automatizados, o que resulta em uma documentação estruturada e consistente
  - Determinar automaticamente um aumento de versionamento semântico (com base nos tipos de commits)
  - Comunicar a natureza das mudanças para colegas de equipe, o público e outras partes interessadas
  - Facilitar a contribuição de outras pessoas em seus projetos, permitindo que eles explorem um histórico de commits mais estruturado
  - O Conventional Commit encoraja a se realizar mais commits de tipos específicos, por exemplo correções
  - A flexibilidade do `Conventional Commits` permite que sua equipe crie seus próprios tipos e altere ao longo do tempo

  ### **Markdown**
  `Markdown` é uma linguagem voltada para *FORMATAÇÃO* de textos. Por exemplo, com ela você não precisa apertar um botão para deixar o texto em *itálico* ou **negrito**.

  Essa linguagem permite formatar e escrever textos usando códigos simples, que não atrapalham a leitura. O maior objetivo do `Markdown` é tornar o texto o mais legível possível. A ideia é que um documento formatado pelo `Markdown` seja publicável como está, como texto simples, sem parecer que foi marcado com *`tags`* ou instruções de formatação.

  Apesar da sintaxe do `Markdown` ter sido influenciada pelas formatações `HTML` existentes, a maior inspiração é o formato de um e-mail simples.

***
### Exercícios 
* [Exercicio para sala](https://github.com/reprograma/on22-b3-s1-git/tree/main/exercicios/para-sala)
* [Exercicio para casa](https://github.com/reprograma/on22-b3-s1-git/tree/main/exercicios/para-casa)

### [Material da aula](https://www.canva.com/design/DAFeHwf3MxE/bhR9Yv9tQm1c3rIX4pkXng/view?utm_content=DAFeHwf3MxE&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)

### Links Úteis

- [Algoritmo e Lógica de Programação](https://dicasdeprogramacao.com.br/o-que-e-algoritmo/)
- [Git](https://git-scm.com/)
- [GitHub](https://github.com/)
- [Commit semânico](https://blog.geekhunter.com.br/o-que-e-commit-e-como-usar-commits-semanticos/)
- [Padrões de commit semântico](https://github.com/iuricode/padroes-de-commits)

- [Sintaxe de Markdown](https://docs.github.com/pt/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)

- [Código limpo](https://balta.io/blog/clean-code#:~:text=Clean%20Code%20ou%20c%C3%B3digo%20limpo,e%20manutenabilidade%20do%20seu%20c%C3%B3digo.) (leitura para mais tarde no curso)



<h1 align="center">
<a href="https://www.instagram.com/_skydoceu/?hl=pt-br"><img src="assets/sky-do-ceu.png"></a>
</h1>

<h2 align="center">
Desenvolvido com :purple_heart:  
</h2>

