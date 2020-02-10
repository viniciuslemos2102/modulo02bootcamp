#  Começo do modulo 2 do bootcamp 08







###  depois de configurado o ambiente com as ferramentas

___

yarn add express

yarn add sucrase -D

yarn add nodemon -D

yarn add editorconfig -D

yarn add eslint -D

yarn add prettier -D

yarn add sequelize

___

###  visualize o packjson.js do arquivo para ver todas as bibliotecas baixadas ate agora

``` js

"scripts": {
    "dev": "nodemon src/server.js",
    "dev:debug": "nodemon --inspect src/server.js"
  },
  "dependencies": {
    "express": "^4.17.1",
    "pg": "^7.18.1",
    "pg-hstore": "^2.3.3",
    "sequelize": "^5.21.4",
    "sequelize-cli": "^5.5.1"
  },
  "devDependencies": {
    "@typescript-eslint/eslint-plugin": "^2.18.0",
    "@typescript-eslint/parser": "^2.19.0",
    "eslint-config-airbnb-base": "^14.0.0",
    "eslint-config-prettier": "^6.10.0",
    "eslint-plugin-import": "^2.20.1",
    "eslint-plugin-prettier": "^3.1.2",
    "nodemon": "^2.0.2",
    "prettier": "^1.19.1",
    "sucrase": "^3.12.1"
  }

  ```

baixe a `docker` [aqui](https://hub.docker.com/ "baixe a docker aqui")

depois de instalada rode o comando :

```
docker run --name database -e POSTGRES_PASSWORD=docker -p 5432:5432 -d postgres:11-alpine
```
depois de instalar o `sequelize-cli` abra o terminal e rode o seguinte comando

```
yarn sequelize migration:create  --name=create-users
```
voce dever ter um retorno parecido com esse

```

Sequelize CLI [Node: 13.7.0, CLI: 5.5.1, ORM: 5.21.4]

migrations folder at "D:\desenvolvimentojs\aulasbootcamp\bootcamp\aulas\modulo02\src\database\migrations" already exists.
New migration was created at D:\desenvolvimentojs\aulasbootcamp\bootcamp\aulas\modulo02\src\database\migrations\20200209234830-create-users.js .
Done in 1.37s.

```
## fala dev! esse é o começo de tudo...estamos quase lá um passo de cada vez...
