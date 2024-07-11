# Install Tools Python

## Install and use Pyenv

    **PYENV-win** 
    1. Ferramenta para gerenciar diferentes versões do Python no Windows.

    
#### Commands
```bash
   Quick start:
    1. Install pyenv-win in PowerShell.
    Invoke-WebRequest -UseBasicParsing -Uri "https://raw.githubusercontent.com/pyenv-win/pyenv-win/master/pyenv-win/install-pyenv-win.ps1" -OutFile "./install-pyenv-win.ps1"; &"./install-pyenv-win.ps1"


```

    Ref.: https://github.com/pyenv-win/pyenv-win

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