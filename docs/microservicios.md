## Inventario de microservicios equipo #1

Este repositorio contiene la información de los microservicios diseñados y realizados por los miembros del equipo

## Tabla resumen
```bash
| microservice-template | plantilla para crear otros microservicios | https://github.com/Diego-3126/microservice-template.git |
| 3.144.194.27 | http://localhost:8080/swagger-ui.html | Diego Fernando España valderrama (Diego-3126) | listo |

| markov-service | Generador de texto automatico (CRUD) | https://github.com/Diego-3126/markov-service.git |
| 3.144.194.27 | http://localhost:8083/swagger-ui.html | Diego Fernando España Valderrama (Diego-3126) | listo |

| asset-service | Subir archivos PDF, videos e imagenes | https://github.com/andresperea01/asset-service |
| 3.144.194.27 | http://localhost:8080/upload.html | Andres David Perea Herrera (andresperea01) | listo |

| auth-service | Inicio de sesion en la plataforma | https://github.com/andresperea01/Auth-service |
| 3.144.194.27 | http://localhost:8081/h2-console | Andres David Perea Herrera (andresperea01) | listo |

| assent-service | registro de usuarios | https://github.com/juanvargas-code/Registro_usuario.git|
| 3.144.194.27 | http://localhost:8080/h2-console | Juan Fernando Vargas Angel (juanvargas-code) | curso |

| list-ovas | listar ovas | https://github.com/SantiagoGonzalezGomez/ms-ovalist.git|
| 3.144.194.27 | http://localhost:8080/h2-console | Santiago Gonzalez Gomez (SantiagoGonzalezGomez) | listo |

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
### microservicio asset-service
```bash
- **Responsable:** Andres David Perea Herrera
- **Repositorio:** https://github.com/andresperea01/asset-service.git
- **Base URL (EC2):**
- **Frontend Upload:** http://localhost:8080/upload.html
- **Swagger UI:** http://localhost:8080/swagger-ui.html
- **H2 Console:** http://localhost:8080/h2-console
- **API Docs:** http://localhost:8080/api-docs
- **Endpoints mínimos:**
  - POST /api/assets - Crear asset con archivo
  - GET /api/assets - Listar todos los assets
  - GET /api/assets/{id} - Obtener asset por ID
  - PUT /api/assets/{id} - Actualizar metadatos
  - PUT /api/assets/{id}/file - Actualizar con archivo
  - DELETE /api/assets/{id} - Eliminar asset
  - GET /api/assets/download/{fileName} - Descargar archivo
  - GET /api/assets/preview/{fileName} - Preview de archivo
  - GET /api/assets/category/{category} - Filtrar por categoría
  - GET /api/assets/limits - Obtener límites de tamaño
  - GET /swagger-ui.html - Documentación Swagger
  - GET /h2-console - Consola base de datos H2

- **Checklist de verificación (semanal):**
  - [✅] Compila y arranca local
  - [✅] `/api/assets` **POST** crea asset con archivo en local
  - [✅] `/api/assets` **GET** lista todos los assets en local
  - [✅] Drag & drop funciona en `/upload.html`
  - [✅] Preview de archivos funciona correctamente
  - [✅] Validación de límites por tipo (PDF: 50MB, Imágenes: 10MB, Videos: 100MB)
  - [✅] Asociación con OVA funcional
  - [✅] Barra de progreso de upload funciona
  - [-] Swagger accesible en EC2
  - [✅] Push diario con commits significativos
  - [✅] Historia/tarea en Jira: **En progreso** → **Terminado** al finalizar
```

### auth-service

```bash
- **Responsable:** Andrés David Perea Herrera
- **Repositorio:** https://github.com/andresperea01/auth-service.git
- **Base URL (EC2):** 
- **Swagger UI:** http://localhost:8081/swagger-ui.html
- **Login Page:** http://localhost:8081/login.html
- **Endpoints mínimos:**
  - POST /api/auth/register
  - POST /api/auth/login
  - GET /api/auth/me
  - GET /swagger-ui.html
  - GET /v3/api-docs

- **Checklist de verificación (semanal):**

  - [✅] Compila y arranca local
  - [✅] `/api/auth/register` y `/api/auth/login` funcionan
  - [-] Swagger accesible en EC2
  - [✅] Push diario con commits significativos
  - [✅] Historia/tarea en Jira: **En progreso** → **Terminado** al finalizar
```

### Assent-servide
```bash
- **Responsable:** Juan Fernando Vargas (Juanvargas-code)  
- **Repositorio:** https://github.com/juanvargas-code/Registro_usuario.git 
- **Base URL (EC2):** 
- **Swagger UI:** http://localhost:8080/swagger-ui.html
- H2 Console: http://localhost:8080/h2-console
- API Docs: http://localhost:8080/api-docs
- Upload Page: http://localhost:8080/upload.html 
- **Entidades principales:**  
  - `<EntidadPrincipal>` (campos clave: …)  
- **Endpoints mínimos:**  
  - `POST /api/register`  
  - `GET /api/user`  
  - `GET /api/upload.html`  
  - `PUT /api/<h2-console`  
   
- **Checklist de verificación (semanal):**  
  - [✅] Compila y arranca local  
  - [✅] `/actuator/health` **UP** en local  
  - [-] Swagger accesible en EC2  
  - [✅] Push diario con commits significativos  
  - [✅] Historia/tarea en Jira: **En progreso** → **Terminado** al finalizar
```
### microservicio Listar-ovas
```bash
- **Responsable:** Santiago Gonzalez Gomez
- **Repositorio:** https://github.com/SantiagoGonzalezGomez/ms-ovalist.git
- **Base URL (Local):** http://localhost:8080
- **Swagger UI:** http://localhost:8080/swagger-ui.html
- **Endpoints**
- `GET /actuator/health`  
- `GET /api/ovas/health`  
- `GET /api/ovas/{id}`  
- `POST /api/ovas`  
- `PUT /api/ovas/{id}`
- `DELETE /api/ovas/{id}`  
- `GET /api/ovas/categoria/{categoria}`
- `GET /api/ovas/buscar?titulo=java`
- **Checklist de verificación (semanal):**  
  - [✅] Compila y arranca local  
  - [✅] `/actuator/health` **UP** en local  
  - [-] Swagger accesible en EC2  
  - [✅] Push diario con commits significativos  
  - [✅] Historia/tarea en Jira: **En progreso** → **Terminado** al finalizar
```
