# chatwoot_local

Este projeto permite subir facilmente, em ambiente **local**, os serviços do **Chatwoot** e da **Evolution API (WhatsApp)** utilizando apenas **Docker Compose**. Não é necessário instalar nada além do Docker e Docker Compose em sua máquina.

## Recursos

- **Chatwoot**: Plataforma de atendimento multicanal.
- **Evolution API**: Integração com WhatsApp.
- Todos os serviços necessários (Postgres, Redis) já configurados.
- Variáveis de ambiente já preenchidas nos arquivos `.env` e `.evo.env`.

## Pré-requisitos

- [Docker](https://docs.docker.com/get-docker/)
- [Docker Compose](https://docs.docker.com/compose/install/)

## Como usar

1. **Clone este repositório:**
   ```sh
   git clone <url-do-repositorio>
   cd chatwoot_local
   ```

2. **Suba os serviços:**
   ```sh
   docker-compose up -d
   ```

3. **Acesse o Chatwoot:**

   [http://localhost:3000](http://localhost:3000)

4. **Acesse a Evolution API:**

   [http://localhost:8080](http://localhost:8080)

---

## Observações

- As variáveis de ambiente já estão configuradas nos arquivos `.env` e `.evo.env`.  
  Caso precise customizar algo, edite esses arquivos **antes** de subir os containers.
- Não é necessário instalar dependências adicionais ou configurar bancos de dados manualmente.

## Para parar os serviços

```sh
docker-compose down
```
