# ReciclApp — Especificación y Arquitectura

Repositorio de documentación arquitectónica del proyecto **ReciclApp**: una plataforma de monitoreo y localización de espacios de reciclaje que permite a ciudadanos consultar el estado (lleno, medio, vacío) y ubicación de contenedores, y a municipalidades gestionar dichos espacios.

## Contenido del repositorio

```
reciclapp-espec/
├── ADR's/               # Decisiones de arquitectura (ADR-1 al ADR-12)
├── Diagramas-C4/        # Diagramas C4 en todos sus niveles
└── Aplicacion-Web.md    # Instrucciones de uso del frontend web
```

## Decisiones de Arquitectura (ADRs)

| ADR | Tema |
|-----|------|
| ADR-1 | Importancia de la usabilidad del sistema |
| ADR-2 a ADR-7 | Decisiones de características del sistema |
| ADR-8 a ADR-9 | Características no funcionales |
| ADR-10 a ADR-11 | Decisiones de estructura |
| ADR-12 | Decisiones de dependencia |

Cada ADR documenta: situación, contexto, decisión tomada, consecuencias y forma de cumplimiento.

## Diagramas C4

| Nivel | Archivo |
|-------|---------|
| Nivel 1 — Contexto | `Diagrama-C4-Nivel_1_Contexto.drawio.png` |
| Nivel 2 — Contenedores | `Diagrama-C4-Nivel_2_Contenedores.drawio.png` |
| Nivel 3 — Componente API | `Diagrama-C4-nivel3_componente_api_app.drawio.png` |
| Nivel 3 — Componente IoT API | `Diagrama-C4-nivel3_componente_iot_api.drawio.png` |
| Nivel 3 — Componente App Mobile | `Diagrama-C4-nivel3_componente_mobile_app.drawio.png` |
| Nivel 3 — Componente App Web | `Diagrama-C4-nivel3_Componente_web_app.drawio.png` |

## Repositorios del proyecto

| Repositorio | Descripción |
|-------------|-------------|
| `reciclapp-api-aplicacion` | API REST backend (NestJS + PostgreSQL + MQTT) |
| `frontend-web` | Aplicación web de administración (Angular) |
| `reciclapp-frontend-app-mobile` | App mobile para ciudadanos (Ionic + Capacitor) |
| `reciclapp-infraestructure` | Infraestructura y despliegue (Docker Compose) |
| `reciclapp-iot-aplicacion` | Firmware del sensor IoT (C++ / PlatformIO) |
