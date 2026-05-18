# Como ejecutar con Docker

Para iniciar la aplicación completa utilizando Docker, simplemente ejecuta:

```bash
docker compose up -d --build
```

Esto va a construir y levantar:
- La **base de datos PostgreSQL** (`db`).
- El **backend** (Node.js + Prisma) que se conecta a PostgreSQL y sincroniza la estructura.
- El **frontend** (Vite + React) servido con Nginx, que actúa como proxy inverso para la API y Socket.io.

Una vez que los contenedores estén levantados, puedes acceder a la aplicación desde cualquier navegador en:
**http://localhost/**

Para detener la aplicación:
```bash
docker compose down
```
