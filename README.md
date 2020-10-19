# Minha primeira CLI

Eu estava curioso, de como, construir uma cli com NodeJS, eu encontrei um post no Medium,
mostrando como criar uma simples CLI.

[Artigo do Medium](https://medium.com/henriquekuwai/criando-sua-cli-com-node-js-d6dee7d03110)

Então vou explicar como funciona, essa simples cli.

# O que é CLI (Command Line Interface)?


A palavra CLI, significa "Command Line Interface", se você é um programador, você deve conhecer CLI's.
São basicamente programas, que permite você usá-los, pelo terminal, prompt de comando. Muitos programas
ficam muito melhores com CLI's, do que com GUI. Por que as CLI's torna em muitas vezes torna o desen-
volvimento mais ágil.

# CLI Criada com base no post do Medium citado acima.

Na cli, foi utilizado alguns módulos, para agilizar no processo de criação de CLI's.

# Módulos :computer:

### Chalk - Para deixar o código colorido.
### Commander - Base muito completa para construção de uma CLI.
### Inquirer - Um agrupador de inputs no CLI (para inputar dados, checkboxes etc.)
### ShellJS - Usado para executar comandos via shell JavaScript.
### FigletJS - Usado para imprimir textos em letras garrafais, pode ser usado com o Chalk.
### Cli Table - para exibir tabelas no terminal.

# Comando para instalar todas essas libs:

`yarn add chalk commander figlet inquirer shelljs cli-table`

# ChalkJS 

Não vai ser necessário, instalar esse módulo, você pode usar o exec ou execSync da lib child_process,
que é uma lib que já vem junto com o NodeJS.

# Todo CLI

Essa foi uma simples CLI, com NodeJS, ele basicamente cria um arquivo que chama todos.json.
Ela não tem utilidade, é só um exemplo simples, para facilitar a compreênsão.

Ele tem alguns comandos:
 `add [todo]`
 `backup`
 `undo <todo>`
 `do <todo>`

## O Comando add [todo]

O comando add, simplesmente adiciona, um "todo", no arquivo todos.json, você pode passar uma flag para 
ele chamada --status ou -s, essa flag é um boolean. A flag --status, é usada para mudar a propiedade
done do objeto gerado "todos.json".

## O comando backup, o comando backup

O comando backup, basicamente, cria uma pasta chamada backup, e guarda todos os to-dos nela.

## O comando list

O comando list é usado para listar todos os to-dos

## O comando undo <todo>

O comando undo é para mudar a propiedade, done para false.

## O comando do <todo>

O comando do é para mudar a propiedade, done para true.

## Autor

👤 **Kaique Araújo**

<h4>Feito com ❤️ e JavaScript.</h3>