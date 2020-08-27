# Desafio Mobile Cross Platform Developer

## Resumo Geral

A idéia desse desafio é entender a capacidade do candidato de resolver problemas de forma simples, criando um CRUD.  
Não temos qualquer interesse em comercializar ou aproveitar de alguma forma o código escrito para esse desafio.

Nossa cultura é focada em resolver problemas de maneira rápida e com a melhor abordagem possivel. Buscamos pessoas que tenham confiança em si e estão dispostas a errar rápido e aprender com os erros.

Leia com atenção todo o conteúdo abaixo sinta-se livre para entrar em contato conosco em caso de dúvidas.
æ
## Estória do Usuário

O Github é uma rede social de programadores que possui uma funcionalidade
interessante que permite curtir o repositório alheio. Trata-se de um botão
escrito Star encontrado na página de cada repositório. Rick é um usuário ativo
do Github, que está sempre buscando novos projetos e curtindo aqueles que são
interessantes. Ele gostaria de poder adicionar um label ou tag para marcar o
repositório de modo que ele possa filtrar. Por exemplo, ele encontrou um
repositório chamado `react` e gostaria de adicionar as tags `javascript` e
`frontend`. Como o Github não possui essa funcionalidade, Rick precisa de um
sistema que consiga ajudá-lo com essa tarefa de um modo simples.

## Sobre o Desafio

O desafio consiste em desenvolver uma aplicação web que obtém todos os
repositórios que um determinado usuário "curtiu". Uma vez obtidos os
repositórios a applicação deve permitir o gerenciamento de tags (adicionar,
editar e remover). Deve ser possivel filtrar os repositórios do usuário pelas
tags. O sistema deve ter um mecanismo de sugestão de tags. Os critérios para
sugestão de tags são de livre escolha do desafiante (linguagem do repositório,
tags atribuidas a outros repositórios, ontras informações disponibilizadas pelo
GitHub, etc).

Requisitos:

 - Recuperar repositórios "starred" do GitHub de determinado usuário.
 - Gerenciar tags dos repositórios recuperados (adicionar, editar, excluir).
 - Filtrar repositórios por tags.
 - Sugestão de tags para os repositorios.

#### Há 4 user stories para entendimento sobre o que é necessário fazer:

##### 1. Obter repositórios remotos

> Como usuário, eu quero fornecer meu username recuperar todos os repositórios
que eu curti para depois conseguir adicionar minhas tags.

* Deve obter os repositórios com star utilizando a API Rest v3 do Github.
* As informações que devem ser recuperadas são: ID do repositório, nome do
repositório, descrição, URL HTTP e linguagem.

##### 2. Adicionar tags para os repositórios

> Como usuário, eu quero poder adicionar tags (labels) para cada repositório
para eu poder efetuar uma busca por tag.

* Um repositório não pode ter tags duplicadas.

##### 3. Buscar repositórios por tag

> Como usuário, quero poder fornecer uma tag e obter os repositórios que possuem
essa tag.

* A busca deve funcionar para consultas com strings pela metade. (ex: ao filtrar
  pela string `doc` tanto repositórios com a tag `docker` quanto com a tag
`documentation` devem ser retornados)

##### 4. Recomendação de tags

> Como usuário, quero receber recomendações de tags para meu repositório.

* Cada repositório deve receber ao menos uma recomendação de tag.

##### Aplicativo

- Deve utilizar React Native ou NativeScript.
- O uso do Redux não é obrigatório mais pode ser utilizado se desejar.
- Os repositórios e suas tags devem ser persistidos em um banco local.
- A interface deve ficar o mais fiel possivel do layout disponibilizado.
- Deve-se manter a organização de código seguindo as boas praticas de desenvolvimento.

## O que vai ser avaliado?

Queremos avaliar sua capacidade em entregar um produto completo e com
documentação mínima suficiente para outros desenvolvedores conseguirem
contribuir com o projeto. É essencial que o `README.md` contenha as intruções
para configurar e rodar o projeto, bastando apenas um ctrl+c/ctrl+v no terminal
do Linux e do OSX para conseguir rodar a aplicação.

Outros pontos que vamos considerar na avaliação:

- Código bem escrito, limpo e coeso.
- Testes automatizados (Cobertura de testes).
- Linter/Análise estática do código.
- README.md bem escrito, curto e com os comandos necessários para rodar a aplicação, bastando copiar/colar no terminal.

## Instruções para entrega

1. Crie um arquivo `README.md` descrevendo como configurar o projeto, contendo os
comandos que devem ser executados para rodar o software e os testes;
2. Suba o projeto no seu github;
3. Disponibilize o link e nos envie a URL por email.

Obs: Se você fez uso de algum Linter, envie o arquivo
de configuração junto com o projeto e descreva qual linter está sendo utilizado no
`README` do projeto.

Qualquer dúvida pode entrar em contato conosco. Boa sorte!
