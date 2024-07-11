# Install Tools Python

## Install and use Pyenv

    **PYENV-win** 
    1. Ferramenta para gerenciar diferentes versões do Python no Windows.

    
#### Commands
```powershell
   Quick start:
    1. Instalacao pyenv-win - PowerShell.

        Invoke-WebRequest -UseBasicParsing -Uri "https://raw.githubusercontent.com/pyenv-win/pyenv-win/master/pyenv-win/install-pyenv-win.ps1" -OutFile "./install-pyenv-win.ps1"; &"./install-pyenv-win.ps1"

    Obs.: Caso comando acima de erro, executar essa linha de comando:

        Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
    

    2. Feche a abra um novo terminal e execute o comando abaixo:
        pyenv --version

    Obs.: Caso o comando acima nao retorne a versao do pyenv, adicione as seguintes variables de ambinte no windows:
        Variable            Value
        PYENV               C:\Users\marcelo\.pyenv\pyenv-win\
        PYENV_HOME          C:\Users\marcelo\.pyenv\pyenv-win\
        PYENV_ROOT          C:\Users\marcelo\.pyenv\pyenv-win\


   Comandos Uteis:
    Verificar versao:
        pyenv --version
    
    Lista as versoes Python suportadas pelo pyenv-win
        pyenv install -l

    Instalar uma versao suportada:
        pyenv install <version>
    
    Setar a versao global pyenv-win
        penv global <version>
    
    Setar a versao local (para um diretorio especifico) pyenv-win
        penv local <version>

    Mostra a versao do python em uso no caminho
        pyenv versions

    Desinstalar uma versao do python
        pyenv uninstall <version>
    




    Ref.: https://github.com/pyenv-win/pyenv-win / 
        
```

#### Como usar
```bash
    Neste exemplo vou configurar a versao 3.11.7 do python, nesse bloco vou instalar a versao 3.11.7 caso ela nao esteja instalada ainda
        pyenv install 3.11.7 

    Para validar 
        pyenv versions

    Entrar no diretorio do projeto
        cd <nome_projeto>

    Seta a versao global do python (Versao padrao do projeto caso informe a versao local)
        pyenv global 3.12.4   # versao corrente instalada na minha maquina

    Seta a versao local a ser utilizada
        pyenv local 3.11.7

    Para validar a versao sendo utilizada no projeto (Caso nao mostre a versao 3.7.11, feche e abrar o novo terminal)
        python --version

    

```

    

## Intall PIP and PIPX

    Utilizados para instalar pacotes e bibliotecas que sera utilizado globalmente no ambiente

## Install Poetry

    O que é a biblioteca Poetry?

    A Poetry é uma ferramenta e biblioteca do Python que foi criada com o objetivo de facilitar o gerenciamento de dependências e a publicação de pacotes. Ele foi desenvolvido para simplificar e melhorar o processo de desenvolvimento Python, oferecendo uma solução completa para tarefas comuns, como:

    1. Gestão de Dependências: Poetry permite que os desenvolvedores definam as dependências de seus projetos de forma clara e concisa. Isso é feito através do arquivo pyproject.toml, que é uma descrição precisa das dependências e configurações do projeto. Ele suporta a especificação de faixas de versões, URLs, arquivos locais e outras fontes de dependências.
    
    2. Isolamento de Ambiente: Poetry cria automaticamente um ambiente virtual para cada projeto, isolando suas dependências e evitando conflitos entre pacotes. Isso garante que as dependências do projeto não entrem em conflito com as de outros projetos.

    3. Gerenciamento de Versões Python: Poetry permite especificar facilmente qual versão do Python seu projeto suporta, garantindo que o ambiente correto seja usado durante o desenvolvimento e a execução.

    4. Empacotamento e Publicação: Uma das características mais destacadas da Poetry é sua capacidade de empacotar e publicar projetos de forma simples e eficiente. Ele cria pacotes compatíveis com PEP 517/518, tornando a distribuição de pacotes Python uma tarefa descomplicada.

    5. Resolução de Dependências Confiável: Poetry usa um algoritmo de resolução de dependências robusto que garante que as versões corretas das dependências sejam instaladas para evitar conflitos e problemas.

    6. Comandos Simplificados: Com uma série de comandos simplificados, como poetry install, poetry add, poetry remove, e poetry publish, Poetry torna as tarefas comuns de desenvolvimento mais fáceis de serem executadas.