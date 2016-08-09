## Depois de entrar na pasta do terminal onde esta localizado o arquivo restaurante.json
## execute o comando mongoimport
mongoimport --db be-mean --collection restaurantes --host=127.0.0.1 --drop --file restaurantes.json

## Ele conectara no db e importara o arquivo JSON
2016-08-09T15:47:48.121-0300	connected to: 127.0.0.1
2016-08-09T15:47:48.125-0300	dropping: be-mean.restaurantes
2016-08-09T15:47:50.101-0300	imported 25359 documents

## contando quanto objetos tem
db.restaurantes.find({}).count()
25359
