## Inventario de microservicios equipo #1

Este repositorio contiene la información de los microservicios diseñados y realizados por los miembros del equipo

## Tabla resumen
```bash
| microservice-template | plantilla para crear otros microservicios | https://github.com/Diego-3126/microservice-template.git |
| 3.144.194.27 | http://localhost:8080/swagger-ui.html | Diego Fernando España valderrama (Diego-3126) | listo |

| markov-service | Generador de texto automatico (CRUD) | https://github.com/Diego-3126/markov-service.git |
| 3.144.194.27 | http://localhost:8083/swagger-ui.html | Diego Fernando España Valderrama (Diego-3126) | listo |
```

## Detalle por servicio

### microservice-template

```bash
- **Responsable:** Diego Fernando España Valderrama (Diego-3126)
- **Repositorio:** https://github.com/Diego-3126/microservice-template.git
- **Base URL (EC2):** 
- **Swagger UI:** http://localhost:8080/swagger-ui.html
- **Endpoints mínimos:**
  - GET /actuator/health
  - GET /api/health
  - GET /swagger-ui.html
  - GET /v3/api-docs
- **Checklist de verificación (semanal):**
 - [✅] Compila y arranca local
 - [✅] `/actuator/health` **UP** en local
 - [-] Swagger accesible en EC2
 - [✅] Push diario con commits significativos
 - [✅] Historia/tarea en Jira: **En progreso** → **Terminado** al
finalizar
```

### markov-service

``` bash
- **Responsable:** Diego Fernando España Valderrama (Diego-3126)
- **Repositorio:** https://github.com/Diego-3126/markov-service.git
- **Base URL (EC2):** 
- **Swagger UI:** http://localhost:8083/swagger-ui.html
- **Entidades principales:**
  - MarkovModel: Entidad principal en base de datos
  - MarkovGenerateRequest: Entrada para generar texto
  - CreateModelRequest: Entrada para crear modelos
  - MarkovGenerateResponse: Salida de generación
  - ModelResponse: Salida de operaciones CRUD
  - ApiResponse<T>: Envoltorio estándar de respuestas
- **Endpoints mínimos:**
  - GET	/api/markov/models
  - GET	/api/markov/models/{id}
  - POST	/api/markov/models
  - PUT	/api/markov/models/{id}
  - DELETE	/api/markov/models/{id}
  - POST	/api/markov/generate
  - GET	/api/markov/health
  - GET	/h2-console
  - GET	/swagger-ui.html
- **Checklist de verificación (semanal):**
 - [✅] Compila y arranca local
 - [✅] `/actuator/health` **UP** en local
 - [-] Swagger accesible en EC2
 - [✅] Push diario con commits significativos
 - [✅] Historia/tarea en Jira: **En progreso** → **Terminado** al
finalizar
```
