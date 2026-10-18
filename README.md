# dados-financeiros

Análise e pipeline sobre dados abertos da CVM (informes diários de fundos) e do Banco Central (séries do SGS).

## Como rodar

1. `cp .env.example .env`
2. `docker compose up -d`
3. `./scripts/baixar_dados.sh`
4. `./scripts/psql.sh -f /sql/ddl/001_raw.sql` e os demais arquivos  `sql/ddl` em ordem
