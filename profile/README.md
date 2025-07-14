# 🏘️ ComuniVeci

Aplicación comunitaria para reportar, aprobar y visualizar problemáticas locales a través de un mapa interactivo y un sistema de participación ciudadana.

🛠️ Proyecto académico – Ingeniería de Software II  
Universidad Nacional de Colombia (2025)

---

## 🌐 Arquitectura distribuida por microservicios

El sistema ComuniVeci se compone de los siguientes módulos:

| Módulo        | Descripción                                                                 |
|---------------|-----------------------------------------------------------------------------|
| 🧩 [`post-service`](https://github.com/ComuniVeci/comuniveci_post_service) | Servicio REST para crear, aprobar, editar y eliminar publicaciones. |
| 🗺️ [`map-service`](https://github.com/ComuniVeci/comuniveci_map_service)   | Servicio de consulta pública de publicaciones aprobadas para el mapa. |
| 💻 [`frontend`](https://github.com/ComuniVeci/comuniveci_front)            | Interfaz gráfica en HTML, CSS y JS puro. Incluye login, perfil y panel admin. |
| 🔐 [`auth-service`](https://github.com/ComuniVeci/comuniveci_auth_service) | Microservicio de autenticación y gestión básica de usuarios con JWT. |
| 📊 [`admin-service`](https://github.com/ComuniVeci/comuniveci_admin_service) | Servicio para métricas, usuarios y estadísticas centralizadas para administradores. |
| 🧪 [`tests`](https://github.com/ComuniVeci/comuniveci_tests)               | Repositorio con pruebas automáticas (frontend y backend) y generación de reportes. |

---

## 🚀 Funcionalidades principales

- ✅ Registro, login y sesión segura con JWT (auth-service)
- ✅ Creación de solicitudes de publicación (frontend → post-service)
- ✅ Aprobación/rechazo de publicaciones por administradores
- ✅ Visualización de publicaciones en un mapa Leaflet.js (map-service)
- ✅ Página de perfil de usuario autenticado
- ✅ Panel de administración con 4 secciones:
  - Publicaciones pendientes
  - Estadísticas de publicaciones
  - Lista de usuarios
  - Métricas Prometheus
- ✅ Diferenciación de roles (usuario vs. administrador)
- ✅ Interacción entre servicios mediante APIs REST

---

## 🧪 Testing y calidad

- Tests de backend con pytest, requests y Faker
- Tests de frontend con Selenium
- Eliminación automática de usuarios de prueba
- Reporte consolidado en PDF de todos los tests (conuniveci_tests)

---

## 👥 Equipo

Este proyecto fue desarrollado como parte del curso Ingeniería de Software II – UNAL 2025 por:

- Julián Vargas y equipo de desarrollo ComuniVeci  
- Docentes y mentores de la Facultad de Ingeniería – Universidad Nacional

---

## 📖 Licencia

Este proyecto se publica con fines académicos y educativos. Puede ser extendido o adaptado libremente bajo los términos de la licencia MIT.

---


