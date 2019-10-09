# Objetivo:
Rodar testes de Iterface do Protheus com TIR - TOTVS Interface Robot, usando Jupyter Notebook

# Motivação:
No Post Web scraping com python —Selenium e Javascript oautor vai fazendo o passo a passo usando jupyter notebook e anaconda.

Então pensei de usar este método para aprender a usar o TIR, e também para implementar no dia a dia.
Se funcionar, o legal é que já dá pra ir criando a documentação, enquanto desenvolve, e reproduzir os passos repetitivos "automágicamente"

Desta forma, todos os passos do estudo ou da atividade já ficam documentados no notebook, e depois é fácil de extrair o código que funciona para gerar os testes automatizados da interface.

Também serve para criar robôs para ferramentas que não tenham como testar sem interface. Como o UPDDISTR e a inicialização da base.

Se acostumar com a rotina também pode ajudar a criar outras ferramentas. 

# Passos para  prototipar:
- [x]Rodar o tutorial do cara com instalação local
- [x]Tentar rodar os scripts de exemplo do TIR
- [x]Ver se funciona sem usar o headless, e ver se tem como rodar só até um ponto, e continuar no env, tipo um repl do python.
- [ ]Com o processo documentado, montar um ou mais artigos com a ferramenta
- [ ]Propor um treinamento pra galeris
- [ ]Rodar no Ubuntu completo (VM)
- [ ]Colocar esta solução no Docker

# Tarefas executadas
- Rodar o tutorial do cara com instalação local
    - [x]Python 3.7
    - [x]pip install pipenv
    - [x] pipenv install jupyter notebook lxml selenium
    - [x]ChromeDriver  -  https://sites.google.com/a/chromium.org/chromedriver/downloads
    - [x]pipenv shell
    - [x]jupyter-notebook
		- [x]Criar um novo notebook e ir executando os comandos
		- [x]Testar sem o headless

- Tentar rodar os scripts de exemplo do TIR: 
    - [x]Rodar um Protheus com WebApp
        - [x]Com Docker - Download do arquivo protheus-dev-sandbox.yml
        - [x]Executar docker-compose -f protheus-dev-sandbox.yml up
    - [x]Instalar o Tir: pip install git+https://github.com/totvs/tir.git --upgrade
    - [x]Baixar os exemplos de https://github.com/totvs/tir-script-samples
    - [x]Executar os exemplos do TIR passo a passo com o Jupyter


## Observações:
- Anaconda - É um atalho para instalar jupyter, pandas e várias coisas de data Science ao mesmo tempo.
- Tentei o Tir no PIPEnv, mas não funcionou - pipenv install -e git+https://github.com/totvs/tir.git#egg=tir
