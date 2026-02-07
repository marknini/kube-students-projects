# Atividade Avaliativa - Deploy de Aplicação em Kubernetes
**Integrantes:** Marknini Toscano Cordeiro e Pedro

## Arquitetura
- **Namespaces:** `app-space` e `db-space`.
- **Backend:** Flask API (2 réplicas) com variáveis via ConfigMap e Secrets.
- **Frontend:** React App (2 réplicas).
- **Banco de Dados:** PostgreSQL via StatefulSet com PVC.
- **Ingress:** NGINX Ingress Controller em http://localhost.

## Como executar
1. `kubectl apply -f namespace.yaml`
2. `kubectl apply -f database/`
3. `kubectl apply -f backend/`
4. `kubectl apply -f frontend/`
5. `kubectl apply -f ingress/`
