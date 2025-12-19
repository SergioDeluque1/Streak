# Documentación del Proyecto Streak

Bienvenido a la documentación completa del proyecto Streak - Plataforma laboral gamificada y marketplace freelance.

## Índice de Documentos

### 📚 Documentos Principales

| Documento                                    | Descripción                                                                                                     | Estado      |
| -------------------------------------------- | --------------------------------------------------------------------------------------------------------------- | ----------- |
| [context.md](./context.md)                   | **Contexto general del proyecto** - Arquitectura completa, modelos de base de datos, tecnologías y convenciones | ✅ Completo |
| [development_plan.md](./development_plan.md) | **Plan de desarrollo paso a paso** - 150+ tareas organizadas en 15 fases para construir el proyecto completo    | ✅ Completo |
| [package-setup.md](./package-setup.md)       | **Configuración del backend** - Dependencias, instalación, configuración de TypeScript, linters y scripts       | ✅ Completo |
| [frontend-setup.md](./frontend-setup.md)     | **Configuración del frontend Flutter** - Dependencias, estructura y configuración de la app móvil               | ✅ Completo |

---

## 🎯 Guía de Uso

### Para Desarrolladores Backend

1. **Inicio:** Lee [context.md](./context.md) para entender la arquitectura completa
2. **Setup:** Sigue [package-setup.md](./package-setup.md) para configurar el entorno
3. **Desarrollo:** Usa [development_plan.md](./development_plan.md) como guía de tareas

### Para Desarrolladores Frontend

1. **Inicio:** Lee [context.md](./context.md) (sección de modelos y API)
2. **Setup:** Sigue [frontend-setup.md](./frontend-setup.md) para configurar Flutter
3. **Referencia:** Consulta [context.md](./context.md) para endpoints y esquemas de datos

### Para Project Managers

1. **Overview:** Lee [context.md](./context.md) para visión general
2. **Planificación:** Consulta [development_plan.md](./development_plan.md) para estimaciones y fases

---

## 📖 Resumen de Cada Documento

### context.md

**Propósito:** Documento maestro del proyecto con toda la arquitectura y especificaciones técnicas.

**Contenido:**

- Descripción general del proyecto
- Stack tecnológico completo
- Estructura de carpetas del backend
- Esquema completo de base de datos (10 colecciones)
- Relaciones entre modelos
- Convenciones de código
- Sistema de gamificación
- Chat y notificaciones
- Reglas para generación de código
- Objetivos y roadmap general

**Cuándo consultarlo:**

- Antes de comenzar cualquier módulo
- Al diseñar nuevas features
- Al definir modelos de datos
- Para revisar relaciones entre entidades

---

### development_plan.md

**Propósito:** Plan de desarrollo secuencial y detallado con tareas atómicas.

**Contenido:**

- 15 fases de desarrollo
- 150+ tareas específicas y verificables
- Metodología: una tarea a la vez
- Checkboxes para seguimiento de progreso
- Fase 0: Configuración inicial (8 tareas)
- Fase 1: Base de datos (4 tareas)
- Fase 2: Middlewares (5 tareas)
- Fase 3-8: Módulos principales (85 tareas)
- Fase 9-12: Features avanzadas (42 tareas)
- Fase 13-15: Workers, testing y deployment (24 tareas)

**Cuándo consultarlo:**

- Diariamente durante el desarrollo
- Para planificar sprints
- Para estimar tiempos
- Para hacer commits organizados

---

### package-setup.md

**Propósito:** Guía completa de configuración del backend Node.js + TypeScript.

**Contenido:**

- Requisitos previos (Node.js, MongoDB, Git)
- Instalación paso a paso
- Todas las dependencias con explicación
- Configuración de TypeScript completa
- ESLint y Prettier configurados
- Scripts de NPM listos para usar
- Variables de entorno (.env.example completo)
- Estructura del proyecto
- Archivos base iniciales
- Troubleshooting común

**Cuándo consultarlo:**

- Al iniciar el proyecto por primera vez
- Al configurar nuevo entorno de desarrollo
- Al agregar nuevas dependencias
- Al resolver problemas de configuración

---

### frontend-setup.md

**Propósito:** Guía de configuración de la aplicación móvil Flutter.

**Contenido:**

- Instalación de Flutter (Windows/Mac/Linux)
- Creación del proyecto
- Dependencias (Riverpod, Dio, Socket.io, etc.)
- Configuración de Firebase
- Estructura de carpetas recomendada
- Configuración de entorno
- Testing
- Scripts útiles
- Troubleshooting

**Cuándo consultarlo:**

- Al iniciar desarrollo del frontend
- Al configurar Firebase
- Al estructurar la app
- Al resolver problemas de Flutter

---

## 🚀 Flujo de Trabajo Recomendado

### Setup Inicial (Primera vez)

```bash
# 1. Backend
cd Streak/streak-backend
# Seguir package-setup.md completamente

# 2. Frontend
cd Streak/streak_app
# Seguir frontend-setup.md completamente

# 3. Verificar documentación
cd Streak/docs
# Leer context.md y development_plan.md
```

### Desarrollo Diario

```bash
# 1. Consultar development_plan.md
# 2. Seleccionar siguiente tarea pendiente
# 3. Consultar context.md para detalles técnicos
# 4. Implementar tarea
# 5. Marcar como completada en development_plan.md
# 6. Commit con mensaje siguiendo convenciones
# 7. Repetir
```

---

## 📝 Convenciones de Commits

Seguir el formato especificado en `context.md`:

```
feat(module): descripción corta

refactor(module): descripción
fix(module): descripción
test(module): descripción
docs: descripción
```

Ejemplos:

```
feat(auth): implement register endpoint with JWT
feat(streaks): add streak calculation service
fix(jobs): resolve pagination issue in getJobs
test(users): add unit tests for UserService
docs: update API endpoints in README
```

---

## 🔄 Actualización de Documentación

Estos documentos son **vivos** y deben actualizarse cuando:

- Se agregan nuevas dependencias → Actualizar `package-setup.md` o `frontend-setup.md`
- Se modifican modelos → Actualizar `context.md`
- Se completan tareas → Marcar en `development_plan.md`
- Se cambia arquitectura → Actualizar `context.md`
- Se descubren mejores prácticas → Actualizar documentos relevantes

---

## 🛠️ Herramientas Recomendadas

### IDEs

- **Backend:** VSCode o Cursor AI
- **Frontend:** VSCode, Android Studio o Cursor AI

### Extensiones VSCode

- ESLint
- Prettier
- REST Client
- MongoDB for VS Code
- Flutter
- Dart
- Error Lens
- GitLens

### Herramientas de Testing

- **Backend:** Jest + Supertest
- **Frontend:** Flutter Test
- **API:** Postman o Thunder Client

### Otras Herramientas

- MongoDB Compass (visualizar DB)
- Postman (testing de API)
- Firebase Console (notificaciones)
- Git (control de versiones)

---

## 📊 Estado del Proyecto

### Backend

- [ ] Configuración inicial
- [ ] Base de datos
- [ ] Sistema de autenticación
- [ ] CRUD de módulos principales
- [ ] Chat y WebSockets
- [ ] Gamificación
- [ ] Notificaciones
- [ ] Workers
- [ ] Testing
- [ ] Deployment

### Frontend

- [ ] Configuración inicial
- [ ] UI/UX básica
- [ ] Autenticación
- [ ] Pantallas principales
- [ ] Chat en tiempo real
- [ ] Notificaciones push
- [ ] Testing
- [ ] Deployment

---

## 🤝 Contribución

### Antes de Codear

1. Leer `context.md` completo
2. Revisar `development_plan.md` para ubicar la tarea
3. Consultar `package-setup.md` o `frontend-setup.md` según corresponda

### Durante el Desarrollo

1. Seguir convenciones de código definidas
2. Documentar código complejo con comentarios
3. Escribir tests para nueva funcionalidad
4. Mantener consistencia con arquitectura existente

### Después de Codear

1. Ejecutar linter y tests
2. Actualizar documentación si es necesario
3. Hacer commit siguiendo convenciones
4. Marcar tarea como completada en `development_plan.md`

---

## 📞 Soporte y Contacto

Si encuentras errores en la documentación o necesitas aclaraciones:

1. Revisa la sección **Troubleshooting** en cada documento
2. Consulta documentación oficial de las tecnologías
3. Abre un issue en el repositorio (si aplica)
4. Contacta al equipo de desarrollo

---

## 📅 Historial de Cambios

| Fecha    | Cambio                                    | Responsable   |
| -------- | ----------------------------------------- | ------------- |
| Oct 2025 | Creación inicial de toda la documentación | Equipo Streak |
| -        | -                                         | -             |

---

## 🎯 Objetivos del Proyecto

### Fase 1 (MVP - 3 meses)

- Sistema de autenticación completo
- CRUD de usuarios, jobs y applications
- Marketplace de gigs básico
- Chat en tiempo real

### Fase 2 (Beta - 6 meses)

- Sistema completo de gamificación
- Notificaciones push
- Workers y tareas programadas
- Sistema de reviews

### Fase 3 (Producción - 9 meses)

- Testing completo
- Optimizaciones de performance
- CI/CD configurado
- Deployment en producción

---

**Proyecto:** Streak - Plataforma laboral gamificada y marketplace freelance

**Empresa:** Magneto

**Stack:** Node.js + TypeScript + MongoDB + Express + Socket.io | Flutter + Riverpod + Firebase

**Última actualización:** Octubre 2025
