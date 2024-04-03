Projeto passo a passo de como usar Sequelize + Migrations

[CMD]
mkdir nome-projeto
cd projeto
code .

npm install --save dotenv
npm install --save sequelize 
npm install --save pg
npm install --save pg-hstore

npx sequelize-cli init

[ARQUIVO]
crie o arquivo .env
NODE_ENV=development

DB_NAME=live
DB_USER=postgres
DB_PASS=postgres
DB_HOST=localhost
DB_PORT=5432
DB_DIALECT=postgres

crie o arquivo .sequelizerc

[CMD]

//cria o banco de dados
npx sequelize-cli db:create

//criar a tabela no banco de dados
npx sequelize-cli migration:generate --name create-clientes

//subir as migracoes para o banco de dados!
npx sequelize-cli db:migrate

//fallback, voce errou e precisa desfazer...
npx sequelize-cli db:migrate:undo

[Links]

[REPOSITORIO](https://github.com/devtvas/node_sequelize)
[VIDEO-AULA](https://www.youtube.com/watch?v=QOKk1PzGLeI&t=1710s)
