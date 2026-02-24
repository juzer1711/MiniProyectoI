# MiniProyectoI
Aplicación web que permite planificar, ejecutar y reprogramar el trabajo asociado a actividades evaluativas1  , así como visualizar su progreso y prioridades sin fricción, especialmente cuando surgen imprevistos (cambios de fechas, acumulación de tareas, sobrecarga semanal).
# 📚 Gestor Inteligente de Actividades Evaluativas

Aplicación web centrada en la experiencia del usuario para planificar, ejecutar y reprogramar actividades evaluativas universitarias, permitiendo visualizar prioridades y progreso sin fricción.

---

## 📖 1. Contexto y Problema

Los estudiantes universitarios necesitan planificar, ejecutar y reprogramar actividades evaluativas (exámenes, tareas, talleres, exposiciones, etc.) especialmente cuando surgen imprevistos como cambios de fecha o sobrecarga semanal.

El problema principal es la falta de una herramienta que:

- Detecte conflictos de carga académica
- Permita replanificación clara
- Muestre prioridades comprensibles para “hoy”
- Visualice progreso real

---

## 🎯 2. Objetivo del Producto

Construir una aplicación web que permita:

1. Crear actividades evaluativas y su plan inicial.
2. Registrar ejecución real.
3. Reprogramar ante conflictos.
4. Visualizar prioridades y progreso en tiempo real.

---

## 🧩 3. Tareas Núcleo (Trazabilidad UX/HCI)

- **T1:** Crear actividad + plan inicial.
- **T2:** Ver prioridades “Hoy”.
- **T3:** Reprogramar y resolver conflicto.
- **T4:** Registrar avance y visualizar progreso.

Cada sprint debe demostrar trazabilidad explícita con estas tareas.

---

## 🚀 4. Alcance Funcional Mínimo (MVP)

Para usuario registrado:

- CRUD de actividades evaluativas.
- CRUD de subtareas con fecha y estimación.
- Vista “Hoy” con reglas de prioridad documentadas.
- Reprogramación con detección de conflicto.
- Registro de avance (hecho/pospuesto).
- Vista de progreso por actividad.

---

## ⚠️ 5. Conflicto Estándar: Sobrecarga Diaria

Se considera conflicto cuando:

La suma de horas estimadas para un día supera el límite definido por el usuario (ej: 6 horas/día).

El sistema debe:

1. Detectar el conflicto.
2. Comunicarlo claramente.
3. Ofrecer alternativas:
   - Mover tarea
   - Reducir estimación
   - Posponer

---

## 🎨 6. Requerimientos No Funcionales (UX/HCI)

El producto será evaluado en:

- Heurísticas de Nielsen.
- Estados del sistema: vacío, cargando, error, éxito.
- Accesibilidad mínima:
  - Navegación por teclado
  - Foco visible
  - Labels correctos
  - Contraste adecuado
  - Mensajes claros
- UX Writing claro y coherente.

---

## 🏗 7. Arquitectura Técnica

### Frontend
- React (SPA)
- Rutas mínimas:
  - /hoy
  - /crear
  - /actividad/:id
  - /progreso
  - /auth

### Backend
- Django REST Framework
- API REST

### Base de Datos
- SQL (Supabase) o
- MongoDB

---

## 🔐 8. Autenticación por Sprints

- Sprint 0–1: Usuario demo permitido.
- Desde Sprint 2: Login obligatorio.
- Protección de rutas.
- Asociación de datos por usuario autenticado.

---

## 🚀 9. Despliegue

- Frontend: Vercel
- Backend API: Render
- URL pública obligatoria al finalizar.

---

## 📊 10. Organización del Equipo

- Tablero Kanban obligatorio:
  - To Do
  - Doing
  - Done
  - Blocked

- Plan semanal por estudiante:
  - 3–5 tareas máximo
  - Definición de terminado
  - Evidencia publicada

Trabajo independiente estimado:
8 horas por estudiante por semana.

---

## 📅 11. Cronograma

- Sprint 0: Setup + prototipo “Hoy” v1.
- Sprint 1: T1 Crear actividad.
- Sprint 2: T2 Vista “Hoy” + Login.
- Sprint 3: T3 Reprogramación + Conflicto.
- Sprint 4: T4 Progreso.
- Sprint 5: UX, accesibilidad y despliegue.
- Semana final: Depuración.

---

## ✅ 12. Definition of Done (DoD)

Una tarea está terminada cuando:

1. Funciona end-to-end (Frontend ↔ API ↔ BD).
2. Tiene estados definidos.
3. Cumple mínimos de accesibilidad.
4. Tiene evidencia publicada.
5. Fue revisada mediante Pull Request.

---

## 👥 13. Roles del Equipo

Los roles son de liderazgo, no de exclusión.

Cada integrante debe:
- Programar
- Publicar evidencia verificable
- Participar en revisión de PRs
- Cumplir su plan semanal

---

## 🧭 14. Reglas de Trabajo con Git

- No trabajar directamente en `main`.
- Usar ramas por funcionalidad:
  - feature/crear-actividad
  - feature/vista-hoy
  - fix/error-login
- Pull Request obligatorio.
- Revisión antes de merge.
- Commits descriptivos:
  - feat:
  - fix:
  - refactor:
  - docs:

---

## 📂 15. Documento Único de Evidencias

Debe contener:

- Link repositorio
- Link tablero Kanban
- Link despliegue
- Capturas por sprint
- PRs
- Endpoints implementados
- Decisiones UX
- Bitácora de iteración
