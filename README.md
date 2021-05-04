# Exercício 00: Mural dos Estudantes 

Professor: João Eduardo Montandon

**Objetivo:** Nesta lista, você irá praticar seus conhecimentos de Git & GitHub para adicionar suas informações no mural dos alunos do curso.
## Mural dos Alunos

O mural dos alunos é uma página que exibe as informações do GitHub de todos que já passaram pela disciplina de DAW ao longo da história do curso.
Você pode acessar essas informações diretamente a partir da página da disciplina, neste [link](https://coltec-daw.github.io/students.html).

Nesta prática, você irá exercitar seus conhecimentos a respeito do Git & GitHub para incluir suas informações no mural da sua turma.


## Clone do projeto

O primeiro passo consiste em fazer uma cópia do projeto para a sua máquina.
Como o projeto está no GitHub (e portanto versionado em git), você poderá usar o comando `$ git clone` para clonar a estrutura do projeto em sua máquina.

**Tarefa: faça o clone do projeto para sua máquina**

### A pasta `_data`

Você vai observar que o projeto contém diversos arquivos.
A grande maioria deles é responsável por fazer o processamento das informações dos alunos e exibí-los automaticamente na página do mural.
Não se preocupe, você não vai precisar alterar nenhum deles! 
Porém, se você tiver interesse em entender como isso é feito, dê uma olhada no [Jekyll](https://jekyllrb.com/).

Nesta atividade, vamos fazer alterações na pasta [`_data`](_data/).
Essa pasta é responsável por armazenar os dos integrantes do mural. 
Repare também que esta pasta contém dois subdiretórios: `students` e `teachers`.
As informações presentes nesse diretório serão processadas pelo Jekyll e então carregadas no arquivo `index.html`.

### O arquivo `jemaf.json`

Ao acessar a pasta `teachers`, você vai observar a presença de um arquivo, chamado [`jemaf.json`](_data/teachers/jemaf.json).
Ao abrir esse arquivo, você vai observar que ele possui a seguinte estrutura: 

```
{
    "introduction": "Olá, jovens!",
    "emoji": "passenger_ship"
}
```

Essas são justamente as informações que serão exibidas no mural!
**Você irá adicionar suas informações em um arquivo próprio, dentro da pasta `students`!**

## Criando o arquivo de seu usuário

Acesse a pasta [`students`](_data/students) e crie um arquivo chamado `USERNAME.json`, **onde `USERNAME` representa seu usuário do GitHub**.

Uma vez criado o arquivo, crie e preencha os campos `introduction` e `emoji`, exatamente como no exemplo acima.
Você pode consultar a lista de emojis disponíveis neste [link](https://emoji-css.afeld.me/).
**ATENÇÃO: Remova o prefixo 'em-' do emoji escolhido (o Jekyll insere esse prefixo automaticamente para você), veja no exemplo acima**.

**Tarefa: Crie um arquivo .json com o nome do seu usuário do GitHub e preencha as informações conforme exemplo acima.**

## Commit e Push

Faça o commit do seu arquivo de usuário com a seguinte mensagem: "Adicionado arquivo referente ao usuário USERNAME".

Em seguida, realize o push das modificações para sincronizá-las com o GitHub.
Se tudo estiver corrido bem, você conseguirá visualizar a página com seu usuário no seguinte link: `https://USERNAME.github.io/E00-Tutorial-Git-GitHub`.

**Tarefa: Faça o commit e push das modificações realizadas no repositório.**

## Entrega

Realize a entrega do trabalho utilizando o mecanismo de pull request.
