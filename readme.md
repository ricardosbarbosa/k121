# k121
Seleção Kenoby

## Clone o projeto com os submodules
`git clone git@github.com:ricardosbarbosa/k121.git --recurse-submodules`

**Importante**: use o comando `--recurse-submodule` para baixar os submodulos do projeto

## Backend

### Configuração do arquivo .env 
#### MongoDB
Forneça a url do banco de dados mongo no formato:
`mongodb://[user]:[senha]@[host]:[port]/[databasename]`

##### MAILGUN
Forneça a _api key_ e o _domain name_ do Mailgun, obtido em _https://app.mailgun.com/app/domains_

**Observação**: Para fins de avaliação desse projeto, o arquivo .env do backend já está preenchido. 
O banco de dados foi provido pelo https://mlab.com.

**ALERTA**: É possivel que o MAILGUN tenha desabilitado minha conta temporariamente. Favor usem os dados de outra conta.

	PORT=3001
	HOSTNAME=127.0.0.1
	DB_HOST=mongodb://admin:adminadmin1@ds121589.mlab.com:21589/k121
	MAIL_GUN_API_KEY=
	MAIL_GUN_DOMAIN=

### Iniciando o servidor localmente
	cd backend
	yarn install 
	yarn start

### Heroku:
Fiz o deploy do backend no heroku: _https://limitless-dawn-76826.herokuapp.com/_

## Frontend

### Configuração do arquivo .env 
Forneça a url de acesso ao backend.

**Observação**: Você encontrá o arquivo .env já preenchido com a url do backend que encontra-se no heroku.

	REACT_APP_BASE_URL_API=https://limitless-dawn-76826.herokuapp.com/

caso prefira usar outro backend mude a url:
	
	REACT_APP_BASE_URL_API=http://localhost:3001 

### Iniciando o servidor localmente
	cd frontend
	yarn install
	yarn start

### Heroku
Fiz o deploy do frontend no heroku: _https://aqueous-woodland-86061.herokuapp.com/_
