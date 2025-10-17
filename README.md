# Desafío Técnico --- Desarrollador Backend Senior (Node.js / NestJS / TypeScript)

### Introducción

Este desafío tiene como objetivo evaluar tus habilidades técnicas en
diseño y desarrollo de APIs escalables, organización de arquitectura
backend, bases de datos relacionales y buenas prácticas en el manejo de
autenticación, modelos y testing.

Tu tarea será construir un **backend funcional** que soporte las mismas
pantallas provistas en el desafío de Frontend (basadas en el Figma
compartido). Este backend deberá proporcionar los **endpoints y lógica
necesarios** para que las páginas puedan consumir datos reales o
simulados desde una API RESTful o GraphQL.

------------------------------------------------------------------------

### Objetivos principales

-   Diseñar y desarrollar una **API estructurada, limpia y mantenible**.
-   Implementar autenticación con JWT (mock o real, a elección).
-   Construir endpoints que permitan alimentar los datos de las
    siguientes vistas:
    1.  Auth -- Sign in
    2.  Project Overview
    3.  Pricing
-   Incluir documentación de la API (Swagger u OpenAPI).
-   Crear una base de datos (PostgreSQL preferido) con modelos
    consistentes.
-   Implementar validaciones, manejo de errores y controladores
    desacoplados.
-   Incluir **tests automatizados** de endpoints y servicios
    principales.

------------------------------------------------------------------------

### Stack técnica requerida

-   Node.js (versión 18 o superior)
-   NestJS (o Express.js con arquitectura modular)
-   TypeScript
-   PostgreSQL (puedes usar SQLite o un mock si prefieres simplificar)
-   ORM: Prisma o TypeORM
-   Autenticación JWT (login + logout + refresh)
-   Swagger u OpenAPI para documentar la API
-   Jest + Supertest para pruebas automáticas
-   Docker para contenedores

------------------------------------------------------------------------

### Endpoints mínimos requeridos

#### 1. Autenticación (`/auth`)

-   `POST /auth/login` → Valida email y contraseña (mock o real).
-   `POST /auth/register` → Crea un usuario nuevo.
-   `GET /auth/profile` → Retorna datos del usuario autenticado.

#### 2. Proyectos (`/projects`)

-   `GET /projects` → Lista de proyectos del usuario.
-   `GET /projects/:id` → Detalle de un proyecto (mock o real).
-   `POST /projects` → Crea un nuevo proyecto.
-   `PATCH /projects/:id` → Actualiza estado o datos del proyecto.

#### 3. Planes (`/pricing`)

-   `GET /pricing` → Retorna los tres planes disponibles (Startup,
    Business, Enterprise).
-   `POST /pricing/select` → Simula la selección de un plan.

------------------------------------------------------------------------

### Testing

Incluye pruebas para las siguientes áreas: - Autenticación (login,
registro, acceso protegido) - CRUD de proyectos - Endpoint de pricing -
Validaciones y manejo de errores

Ejecutar tests:

``` bash
npm run test
```

------------------------------------------------------------------------

### Evaluación

  -----------------------------------------------------------------------
  Criterio                       Descripción
  ------------------------------ ----------------------------------------
  Arquitectura                   Organización modular y separación de
                                 responsabilidades

  Código limpio                  Uso correcto de TypeScript,
                                 convenciones, ESLint, Prettier

  Documentación                  Swagger, README, ejemplos de uso

  Testing                        Cobertura de pruebas y claridad de los
                                 casos

  Seguridad                      Buenas prácticas en autenticación y
                                 manejo de datos

  Performance                    Eficiencia y uso de asincronía

  Escalabilidad                  Capacidad de extender la API fácilmente
  -----------------------------------------------------------------------

------------------------------------------------------------------------

### Entrega

1.  Crea un repositorio público en GitHub con el nombre
    **lianzo-backend-challenge**.

2.  Incluye un `README.md` explicando tu arquitectura y decisiones
    técnicas.

3.  Incluye el script para levantar el proyecto:

    ``` bash
    npm install
    npm run start:dev
    ```

4.  Incluye la documentación Swagger accesible en `/api/docs`.

5.  Envía el enlace del repositorio al correo:
    **kalebeoliveira.dev@gmail.com**

------------------------------------------------------------------------

### Recursos

Figma (referencia visual): [Link
Figma](https://www.figma.com/design/z7BEqnLA2Xt0qTGp1VXwGT/Sem-t%C3%ADtulo?node-id=0-1&t=Au4uXA3gLcszcxVb-1)

------------------------------------------------------------------------

### Contacto

Si tienes dudas, puedes contactar al equipo técnico de **Lianzo**:
kalebeoliveira.dev@gmail.com

¡Buena suerte y demuestra tu mejor arquitectura backend!
