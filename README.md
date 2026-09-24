# DeepSeek V4 Flash API (deepseek-v4-flash / deepseekv4flash) — llm guide with published pricing

> **input $0.3429; cached_input $0.0686; output $1.0286** — flat per-unit billing through the OpenAI-compatible APIMart gateway, $1 minimum top-up.

**[Live pricing](https://apimart.ai/pricing)** · **[Get an API key](https://apimart.ai/keys)**

Everything here refers to **deepseek-v4-flash** — also written **deepseekv4flash** or **deepseek v4 flash**.

## Pricing (observed, snapshot 2026-09-24)

| Tier | Price |
| --- | --- |
| `input` | $0.3429 |
| `cached_input` | $0.0686 |
| `output` | $1.0286 |

## Cost at scale

| Volume | Cost |
| --- | --- |
| 100 | $34.2857 |
| 1,000 | $342.8568 |

## How to call it

```bash
curl --request POST --url https://api.apimart.ai/v1/images/generations \
  --header "Authorization: Bearer $APIMART_API_KEY" --header 'Content-Type: application/json' \
  --data '{"model":"deepseek-v4-flash","prompt":"a modern cliffside villa at dusk","size":"16:9","n":1}'
```

Submit, keep the `task_id`, poll `GET /v1/tasks/{id}` until `completed`; the response carries the URL and the exact amount charged.

## Disclosure

Documents access through APIMart, a third-party API gateway; not affiliated with the model vendor.
