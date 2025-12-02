# Linka

MVP stack: Go, PostgreSQL, Redis, WebSockets, React.

Services
- gateway: REST + WebSocket

Infra (dev)
- PostgreSQL
- Redis
- MinIO (S3-compatible)
- Meilisearch

Quick start
1) Copy deploy/.env.example to deploy/.env and set variables
2) docker compose -f deploy/docker-compose.yml --env-file deploy/.env up -d --build

HTTP base: http://localhost:8080
WebSocket: ws://localhost:8080/ws?token=JWT

Endpoints
- POST /v1/auth/signup
- POST /v1/auth/login
- POST /v1/messages/send
- GET  /v1/messages/with/{user_id}

Do not share secrets publicly. Rotate credentials after testing.

# linka_mobile

A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://docs.flutter.dev/cookbook)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.
