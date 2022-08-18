<h1 align="center"> DEVinventory </h1>

## Empresa

<p>A empresa responsável pelo projeto é a M2P2 Software Ltda e o squad responsável pelo desenvolvimento é a equipe Black Mirror.</p>

## Tópicos

- [Descrição do projeto](#descrição-do-projeto)
- [Realização do projeto](#realização-do-projeto)
- [Funcionalidades](#funcionalidades)
- [Como executar](#como-executar)
- [Endpoints](#endpoints)
- [Desenvolvedores](#desenvolvedores)
- [Tecnologias utilizadas](#tecnologias-utilizadas)

## Descrição do projeto
<p align="justify">
 Este é o segundo projeto do módulo 2 do curso DEVinHouse do Serviço Nacional de Aprendizagem Industrial - SENAI em parceria com o LAB365 e a empresa Conecta Nuvem. A proposta deste projeto é a construção de uma API com sistema backend de cadastro e empréstimos de itens das empresas para seus funcionários.
 A proposta tem como base um arquivo com requisitos da aplicação e contém um modelo de entidade relacionamento para construção do banco de dados através da utilização das tecnologias python, SQL, postgresql e flask.
</p>

## Realização do projeto
<p align="justify">
 O desenvolvimento foi realizado em grupo simulando o dia-a-dia de uma empresa do ramo de tecnologia através das metodologias ágeis. Utilizamos a metodologia scrum, onde nosso squad é formado por 7 desenvolvedores full stack e o product owner é o professor da turma.
</p>
<p align="justify">
 No primeiro dia nos praparamos em uma sprint planning juntamente com a sprint backlog (visto o prazo curto), definindo o formato dos commits, nomes de branchs, realização dos pull requests, taks, e ferramenta para organização do desenvolvimento. Para realização das atividades definimos utilizar o trello, separando os cards como tasks, onde cada desenvolvedor está livre para escolher sua task e arrastar entre os campos definidos na ferramenta, lembrando sempre de deixar o card no campo 'code review' enquanto o pull requst estiver sendo testado.
</p>
<p align="justify">
 Todos os dias fizemos a daily, repassando o que foi desenvolvido e se houveram dificuldades. Como o prazo para entrega é curto, todos ajudavam quando ocorria alguma dificuldade entre os desenvolvedores.
</p>

![imagem_2022-08-18_104446081](https://user-images.githubusercontent.com/101053966/185410294-83c9b492-d931-47bb-8247-09bc27997d17.png)

## Funcionalidades

✔️ `Login:` Efetuar login no sistema.

✔️ `Login/Cadastro:` Efetuar login com uma conta google.

✔️ `Cadastro:` Realizar cadastro dos colaboradores da empresa.

✔️ `Cadastro:` Realizar o cadastro de itens no inventário.

✔️ `Emprestimo:` Realizar o empréstimo de itens para os colaboradores.

✔️ `Contagem:` Efetuar a contagem de itens emprestados, total de itens cadastrados, soma dos valores totais de todos os itens e total de colaboradores cadastrados.

✔️ `Atualização:` Efetuar a atualização dos dados do colaborador e/ou itens quando necessário.

## Como executar

- Primeiramente você precisará ter instalado em sua máquina: **Python 3.10**, **Poetry**, **Postgresql** e uma plataforma de sua preferência: pgAdmin, DBeaver ou outro.
<p align="justify">
    Para instalação utilizar:
</p>

Python:
```
https://www.python.org/downloads/windows/
```
```
https://python.org.br/instalacao-linux/
```
Poetry:
* osx / linux / bashonwindows install instructions
```
curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python -
```
* windows powershell install instructions
```
(Invoke-WebRequest -Uri https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py -UseBasicParsing).Content | python -
```
Postgresql:
```
https://www.postgresql.org/download/
```
`Sugestão`: pgAdmin:
```
https://www.pgadmin.org/download/
```

Em seguida você precisará executar os comandos a seguir para criar o ambiente virtual local, ativá-lo e instalar as dependências do projeto:

```
poetry config --local virtualenvs.in-project true
```
```
.\.venv\Scripts\activate
```
```
poetry install
```
<p align="justify">
 A seguir você precisará criar um arquivo de variáveis de ambiente chamado *.env*. Para isso você utilizará como exemplo o arquivo *.env_example*, apenas trocando os dados de exemplo para os dados que você irá utilizar em sua máquina para testes.
</p>

Feito isso, você irá utilizar os comandos a seguir para criar suas tabelas:

```
poetry run flask db init
```
```
poetry run flask db migrate
```
```
poetry run flask db upgrade
```
Para ter alguns dados no banco e manipulá-los:
```
poetry run flask populate_db
```
`OBS`: Caso precise, pode utilizar o comando **_poetry run flask drop_all_tables_** para retirar todas as tabelas do banco e recomeçar novamente (não sendo necessário o comando 'poetry run flask db init'). 

## Endpoints
1.
2.
3.
4.
5.
6.
7.
8.
9.
10.

## Tecnologias utilizadas

<p align="left"> 
<a href="https://flask.palletsprojects.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/pocoo_flask/pocoo_flask-icon.svg" alt="flask" width="40" height="40"/> 
</a> 
<a href="https://www.sqlalchemy.org" target="_blank" rel="noreferrer"> <img src="https://butecotecnologico.com.br/comecando-com-sql-alchemy/sql-alchemy-logo_hu9aaae5cb0138810bd2a9b3020b120bcf_12170_200x200_resize_q90_bgffffff_linear_2.jpg" alt="sqlalchemy" width="40" height="40"/> 
</a> 
<a href="https://www.sqlalchemy.org" target="_blank" rel="noreferrer"> <img src="https://cdn-icons-png.flaticon.com/512/2772/2772165.png" alt="sql" width="40" height="40"/> 
</a> 
<a href="https://flask-marshmallow.readthedocs.io/en/latest/" target="_blank" rel="noreferrer"> <img src="https://w7.pngwing.com/pngs/1009/741/png-transparent-python-serialization-object-marshmallow-database-marshmellow-angle-white-face-thumbnail.png" alt="marshmallow" width="40" height="40"/> 
</a> 
<a href="https://git-scm.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/git-scm/git-scm-icon.svg" alt="git" width="40" height="40"/> 
</a> 
<a href="https://www.postgresql.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/postgresql/postgresql-original-wordmark.svg" alt="postgresql" width="40" height="40"/> 
</a> 
<a href="https://www.python.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/> 
</a> 
</p>

## Desenvolvedores

| [<sub>Breno Martins</sub><br><img src="https://avatars.githubusercontent.com/u/95316873?v=4" width=100><br>](https://github.com/Breno-MT) | [<sub>Luiz Gustavo Seeman</sub><br><img src="https://avatars.githubusercontent.com/u/101838119?v=4" width=100><br>](https://github.com/Gustavo-Seemann) | [<sub>Marcelo Coelho</sub><br><img src="https://avatars.githubusercontent.com/u/92119579?v=4" width=100><br>](https://github.com/MCoelho222) | 
| :---: | :---: | :---: |
| [<sub>Rafael Telles Carneiro</sub><br><img src="https://avatars.githubusercontent.com/u/98103640?v=4" width=100><br>](https://github.com/rafatellescarneiro) | [<sub>Josinaldo Andrade Pereira</sub><br><img src="https://avatars.githubusercontent.com/u/101839277?v=4" width=100><br>](https://github.com/josinaldoandradepereira) | [<sub>Thiago William</sub><br><img src="https://avatars.githubusercontent.com/u/94487053?v=4" width=100><br>](https://github.com/ThiagoW21) | 
[<sub>Vinicius Possatto Stormoski</sub><br><img src="https://avatars.githubusercontent.com/u/101053966?v=4" width=100><br>](https://github.com/ViniciusPosssatto)