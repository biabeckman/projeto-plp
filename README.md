<h1 align="center"> CODEFIT </h1>

O CODEFIT, é um sistema de gerenciamento de academia que pode ser utilizado por gestores, funcionários e alunos. O sistema contém funcionalidades específicas para cada usuário visando modularizar o sistema, atribuindo cada funcionalidade a entidade específica.

# Tecnologias Utilizadas
- [Haskell](https://www.haskell.org) : programação funcional
- [Prolog](https://www.swi-prolog.org) : programação lógica

# Índice 
* [Índice](#índice)
* [Tecnologias utilizadas](#tecnologias-utilizadas)
* [Funcionalidades](#funcionalidades)
* [Rodando em Prolog](#rodando-localmente-em-prolog)
* [Rodando em Haskell](#rodando-em-haskell)

# Tecnologias Utilizadas
- [Haskell](https://www.haskell.org) : programação funcional
- [Prolog](https://www.swi-prolog.org) : programação lógica

# Funcionalidades

- Conheça todas as funcionalidades disponíveis acessando a [documentação oficial do projeto](https://docs.google.com/document/d/1bcGVitOdJ7p6JWy1ikgXhyCYMsLPlYAsG7g90WwrG-o/edit#heading=h.phrzmz7sb5x0). 

- Vídeo de apresentação do CODEFIT:[Sistema CODEFIT](https://youtu.be/EZQIBaNyYaw).


# Rodando localmente em Prolog

### Cuidado!
É preciso que você tenha o SWI Prolog instalado e atualizado em sua máquina.
Caso não tenha o swi, 
  esse vídeo irá lhe ensinar detalhadamente [instalação swi](https://www.youtube.com/watch?v=YzDpQOk2qvQ).
E logo após, também, deve ser baixado uma pack, abaixo segue as instruções de como baixar:

Insira no terminal do seu computador
```bash
  swipl
```
Se estiver instalado, e aparecer ?-
```bash
  pack_install(smtp).
  // escolha o diretório e depois a letra Y
```

Tudo pronto? Vamos em frente!

##Para rodar as classes, siga as instruções abaixo

Clone o projeto em sua IDE

```bash
  git clone [https://github.com/kevinicolas22/projeto-plp-prolog.git]
```
Verifique se está na branch 'main', se não tiver insira : git checkout main

-> Entre no diretório do projeto

```bash
  cd prolog
```

-> Para rodar o menu principal

```bash
  swipl -q -f mainPrincipal.pl
```
-> Para rodar apenas gestor
```bash
  swipl -q -f mainGestor.pl
```
```bash
  menu_gestor(MenuPrincipal).
```
-> Para rodar apenas funcionario
```bash
  swipl -q -f mainFuncionario.pl 
```
```bash
  menu_funcionario.
```
-> Para rodar apenas aluno
```bash
  swipl -q -f mainAluno.pl
```
```bash
  login_aluno.
```

# Rodando em Haskell 
### Cuidado!
É preciso que você tenha o Cabal instalado e atualizado em sua máquina.
Caso não tenha o cabal, essas informações vão te ajudar...

Cole em seu terminal
```bash
  Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; try { Invoke-Command -ScriptBlock ([ScriptBlock]::Create((Invoke-WebRequest https://www.haskell.org/ghcup/sh/bootstrap-haskell.ps1 -UseBasicParsing))) -ArgumentList $true } catch { Write-Error $_ }
```
Em caso de dúvidas acompanhe o vídeo:
```bash
  [https://youtu.be/bB4fmQiUYPw?feature=shared]
```

Tudo pronto? Vamos em frente!

Clone o projeto em sua IDE

```bash
  git clone [https://github.com/kevinicolas22/projeto-plp.git]
```

Entre no diretório do projeto

```bash
  cd haskell
```

Gerar arquivo .cabal

```bash
  cabal init
```
Instalar dependências

```bash
  cabal build
```

Execute o programa com

```bash
  cabal run
```

Ainda é possível que o programa apresente erros porque você não está com o cabal devidamente atualizado. Atualize-o com o comando abaixo e tente novamente.
```bash
  cabal upgrade
```

