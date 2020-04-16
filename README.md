# node-depoy
Deploy de aplicações NodeJS à AWS com Docker

### Comandos Usados...

#### criar instância
docker-machine create --driver amazonec2 aws01
#### informações da instância
docker-machine env aws01
#### comandos direto na instância
eval $(docker-machine env aws01)
#### remover comandos direto da instância
eval $(docker-machine env -u)
#### enviando dados para instância
docker-compose -f docker-compose.yml -f docker-production.yml up -d
#### regerando acesso a instância
docker-machine regenerate-certs aws01
