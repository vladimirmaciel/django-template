## Backend Django 
Nesta pasta encontra-se os arquivos de backend do projeto Django.

Será utilizado o Poetry para gerenciar as dependências do projeto. Para instalar o Poetry, execute o comando abaixo:
### Obs.: Verifique se tem o pyenv instalado, rode o comando `pyenv with python`
 1 - Instale o Poetry:
```bash
pip install poetry
```
 2 - Incialize o Poetry:
```bash
poetry init
```
 3 - Configure o Poetry para criar o ambiente virtual na pasta `.venv`:
```bash
poetry config virtualenvs.in-project true
```
 4 - Instale as dependências do projeto:
```bash
 poetry add django
```

5 - Para instalar o projeto, dentro da pasta backend, execute o comando:
```bash
poetry install --sync
```
O comando `poetry install --sync` sincroniza as dependências do projeto com o arquivo `pyproject.toml`. Ele remove qualquer dependência que não esteja listada no arquivo e instala as que estão listadas, garantindo que o ambiente esteja exatamente como especificado.
6- Ative o ambiente virtual:
```bash
poetry shell
```
7 - Crie o projeto Django:
```bash
django-admin startproject mysite
```
8 - Execute o servidor:
```bash
python manage.py runserver
```

9 - Instalar depedenicas do projeto de desenvolvimento pytest e pytest-django  com  -G dev:

```bash
poetry add pytest pytest-django -G dev
```