## Descrição

Repositório do Apache Kafka (Mensageria)

**Importante**: Roda-lo antes de qualquer aplicação

## Configurar /etc/hosts

A comunicação entre as aplicações se dá de forma direta através da rede da máquina.
Para isto é necessário configurar um endereços que todos os containers Docker consigam acessar.

Acrescente no seu /etc/hosts (para Windows o caminho é C:\Windows\system32\drivers\etc\hosts):

```
127.0.0.1 host.docker.internal
```

Em todos os sistemas operacionais é necessário abrir o programa para editar o _hosts_ como Administrator da máquina ou root.

## Rodar a aplicação

Execute os comandos:

```
docker-compose up
```

**_Importante_**: Toda vez que para-lo de rodar, rode `docker-compose down` para destruir os volumes, senão ao rodar um UP novamente dará erro
