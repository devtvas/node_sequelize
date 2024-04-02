[LINK REPOSITORIO](https://github.com/devtvas/node_sequelize)

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

npx sequelize-cli db:create
