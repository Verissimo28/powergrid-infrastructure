# PowerGrid Infrastructure

Infraestrutura local do projeto PowerGrid.

## Serviços

- `core-db`: PostgreSQL exclusivo do Core;
- `audit-db`: PostgreSQL exclusivo do Audit;
- `redis`: estado e presença do Live;
- `rabbitmq`: comunicação assíncrona entre serviços.

## Inicialização

```bash
cp .env.example .env
docker compose config
docker compose up -d
docker compose ps