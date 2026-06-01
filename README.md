# uni-observ

Observability стек для моніторингу всіх сервісів. Включає Grafana, Prometheus, Loki, Tempo та OpenTelemetry Collector.

## Компоненти

| Інструмент | Призначення |
|---|---|
| Grafana | Дашборди та візуалізація |
| Prometheus | Метрики |
| Loki | Логи |
| Tempo | Трейсинг |
| OTEL Collector | Збір та роутинг телеметрії |

## Запуск

```bash
# Спільна мережа (один раз, якщо ще не створена)
docker network create uni-net

docker compose up -d
```

Запускайте цей стек **першим**, до запуску інших сервісів.

## Дашборди

| Сервіс | URL |
|---|---|
| uni-logium-svc | `http://localhost:3000/d/logium-svc` |
| uni-products-svc | `http://localhost:3000/d/products-svc` |
