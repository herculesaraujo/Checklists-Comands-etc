###   Listar containers
```js
docker -v
```

###   Ver comandos disponíveis
```js
docker --help
```

###   Listar containers no Docker (na Matrix)
```js
docker ps [-a | --all]
```
```js
docker container ps [-a | --all]
```
```js
docker container ls [-a | --all]
```
```js
docker container list [-a | --all]
```
###   Criar um container (Jogar indivíduo na Matrix!)

```js
  docker run
```
###  Criando um container sem executar
```js
  docker create -it 
```
```js
  docker start 
```
### 7. Entrando em um container já em execução 
```js
  docker container attach 
```

### 8. Criando contêiner em segundo plano
```js
  docker container run -tid ubuntu
```
### 9. Parando um contêiner
```js
  docker stop 
```
### 10. Iniciando um contêiner parado
```js
  docker start 
```
### 11. Reiniciar contêiner 
```js
  docker restart 
```
### 12. Pausar um contêiner
```js
  docker pause 
```
### 13. "Despausar" um contêiner
```js
  docker unpause 
```
### 14. Remover contêiner 
```js
  docker rm 
```
### 15. Remove contêiner parados
```js
  docker container prune
```

```js
  docker rm $(docker ps -a -q)
```
### 15. Remove Todos os contêiner ( parados ou não )
```js
  docker rm -f $(docker ps -aq) 
```
   Obs: -f: força remoção dos em execução
   -q: não mostar o retorno da lista, apenas ID
   

### 15. Remove Todos as imagens
```js
  docker rmi $(docker images -q)
```
   -q: não mostar o retorno da lista, apenas ID
   
   
