# Guia de Comandos

## Introdução

Este documento visa fornecer um compilado de comandos Linux e Git para aprendizado e revisão, contendo a sintaxe do comando e uma explicação simples da funcionalidade. O documento poderá ser atualizado para incluir mais comandos, a depender da necessidade dos autores.

## Sumário

- [Comandos Linux](#linux)
  - [cd](#cd-diretório)
  - [ls](#ls)
  - [mkdir](#mkdir-diretório)
  - [rm](#rm-arquivodiretório)
  - [cp](#cp-origem-destino)
  - [mv](#mv-origem-destino)
  - [touch](#touch-arquivo)
  - [cat](#cat-arquivo)
  - [nano](#nano-arquivo)
  - [curl](#curl-url)
  - [sudo/apt](#sudoapt)
- [Comandos Git](#git)
  - [add](#add-arquivo)
  - [status](#status)
  - [commit](#commit--m-mensagem)
  - [push](#push)
  - [pull](#pull)
  - [fetch](#fetch)
  - [remote](#remote)
  - [branch](#branch)

## Linux

### cd {diretório}

Muda o diretório atual, informando o diretório ou o caminho para o diretório.

- Utilize `.` para referenciar o diretório atual;
- Utilize `..` para referenciar o diretório anterior.

### ls

Lista os arquivos no diretório atual.

- Utilize a opção `-l` para listar de maneira mais detalhada;
- Utilize a opção `-a` para listar arquivos ocultos.

### mkdir {diretório}

Cria um diretório, podendo ser na pasta atual ou indicando o caminho em que o diretório ficará.

### rm {arquivo/diretório}

Remove arquivos ou diretórios.

- Utilize `-r` para remover diretórios recursivamente;
- Utilize `-f` para forçar a remoção sem confirmação.

### cp {origem} {destino}

Copia arquivos ou diretórios.

- Utilize `-r` para copiar diretórios recursivamente.

### mv {origem} {destino}

Move ou renomeia arquivos e diretórios.

### touch {arquivo}

Cria um novo arquivo vazio.

### cat {arquivo}

Exibe o conteúdo de um arquivo no terminal.

### nano {arquivo}

Abre o editor de texto `nano` para editar o arquivo especificado.

### curl {URL}

Faz requisições HTTP e baixa arquivos da internet.

- Utilize `-o {nome_do_arquivo}` para salvar o conteúdo em um arquivo.

### sudo/apt

- `sudo {comando}`: Executa um comando com permissões de superusuário.
- `apt update`: Atualiza a lista de pacotes disponíveis.
- `apt upgrade`: Atualiza os pacotes instalados no sistema.
- `apt install`: Instala os pacotes informados.

## Git

### add {arquivo}

Adiciona um arquivo ao staging area (prepara para commit).

- Utilize `.` para adicionar todos os arquivos modificados.

### status

Mostra o status atual do repositório Git.

### commit -m "mensagem"

Registra as alterações no repositório.

### push

Envia os commits locais para o repositório remoto.

- O primeiro commit de uma nova branch deve ser `git push --set-upstream origin {branch}`

### pull

Atualiza o repositório local com as alterações do repositório remoto.

### fetch

Baixa as alterações do repositório remoto, mas não as mescla automaticamente.

### remote

Gerencia os repositórios remotos.

- `git remote -v`: Lista os repositórios remotos configurados.
- `git remote add {nome} {URL}`: Adiciona um novo repositório remoto.

### branch

Gerencia as branches do repositório.

- `git branch`: Lista as branches existentes.
- `git branch {nome}`: Cria uma nova branch.
- `git checkout {nome}`: Alterna para a branch especificada.
