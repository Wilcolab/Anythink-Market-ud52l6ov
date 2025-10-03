
# Anythink Market - Multi-server Project

Este proyecto contiene dos servidores:

- **Python FastAPI** (puerto 8000)
- **Node.js Express** (puerto 8001)

Ambos servidores gestionan una lista de tareas y exponen endpoints similares.

## Estructura del Proyecto

- `python-server/src/main.py`: Implementación del servidor FastAPI.
- `express-server/src/index.js`: Implementación del servidor Express.
- `docker-compose.yml`: Orquestación de ambos servicios con Docker Compose.

## Cómo ejecutar ambos servidores

1. Construye y levanta los contenedores:

  ```bash
  docker compose up
  ```

2. Accede a los servidores:
  - Python: http://localhost:8000
  - Node.js: http://localhost:8001

## Endpoints disponibles

### Python FastAPI (puerto 8000)
- `POST /tasks`: Agrega una tarea.
- `GET /tasks`: Devuelve la lista de tareas.

### Node.js Express (puerto 8001)
- `POST /tasks`: Agrega una tarea.
- `GET /tasks`: Devuelve la lista de tareas.
- `GET /`: Devuelve "Hello World".
