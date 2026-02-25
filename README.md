# Arquitectura de Software — 2026-1

Repositorio de laboratorios de la asignatura **Arquitectura de Software** del semestre 2026-1 de la **Universidad Nacional de Colombia**.

## Contenido

| Laboratorio | Descripción | Tecnologías |
|-------------|-------------|-------------|
| [Laboratorio 1](./Laboratory%201/swarch/) | Aplicación web para gestión de calificaciones con arquitectura en capas (MVC) desplegada mediante Docker | Python · Flask · MySQL · Docker |

## Estructura del repositorio

```
Arquisoft-2026-2/
└── Laboratory 1/
    └── swarch/          # Aplicación Flask + MySQL (gestión de calificaciones)
        ├── app.py
        ├── config.py
        ├── controllers/
        ├── models/
        ├── repositories/
        ├── services/
        ├── templates/
        ├── Dockerfile
        ├── docker-compose.yml
        └── requirements.txt
```

## Laboratorio 1 — Gestión de Calificaciones

Aplicación web con arquitectura en capas (MVC) que permite registrar, listar y eliminar calificaciones de estudiantes.

### Requisitos previos

- [Docker](https://docs.docker.com/get-docker/) (versión más reciente)
- [Docker Compose](https://docs.docker.com/compose/install/) (versión más reciente)

### Ejecución

```bash
cd "Laboratory 1/swarch"
docker compose up --build
```

La aplicación estará disponible en [http://localhost:8080](http://localhost:8080).

### Ejecución local (sin Docker)

Requisitos adicionales: Python 3.11+ y MySQL 5.7+.

```bash
cd "Laboratory 1/swarch"
pip install -r requirements.txt
python app.py
```

> Asegúrate de configurar las credenciales de la base de datos en `config.py` antes de ejecutar la aplicación localmente.

## Licencia

Este proyecto está licenciado bajo la [Licencia MIT](./LICENSE).
