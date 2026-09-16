# schema-dados-branchs

Schema de dados da API de registros de vendas, versionado por branch.

## Estrutura

| Arquivo | Descrição |
|---|---|
| `schema_dados.json` | JSON Schema (draft 2020-12) do payload da API |

## Branches

- `main` — versão estável
- `feature-*` — alterações em desenvolvimento, entram via Pull Request

## Payload

```json
{
  "nome_squad": "DataEngineers",
  "versao_api": "1.0",
  "data_coleta": "2026-09-15",
  "registros_vendas": [
    {
      "id_transacao": 1001,
      "cliente": "Empresa ABC",
      "valor_total": 1550.50,
      "status_qualidade": "VALIDO",
      "campos_nulos": 0
    }
  ]
}
```

`status_qualidade` aceita `VALIDO`, `ATENCAO` ou `INVALIDO`.
