# Prometheus

## Problema
- Arquitetura de containers e microserviços;
- Complexidade e dificuldade em observar a saúde do sistema
- Db fail, auth server fail, app fail, erro 503 -> onde foi o problema?

## Arquitetura
![Arch](./prometheus-server.png)

Prometheus Server
- Retrieval
Puxa as métricas dos serviços, aplicações, servidores e joga pro storage
- Storage
Guarda as métricas em um Time Series Database
- HTTP Server
Aceita as queries no formato PromQL