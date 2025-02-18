# Historias de Usuario – Gestión de Reclutamiento

## 🧑‍💼 User Story 1: Gestión de Candidatos  

### 🎯 Título: Crear y gestionar candidatos desde la interfaz de reclutador  

- **Como:** Reclutador de Recursos Humanos  
- **Quiero:** Agregar, actualizar, buscar y gestionar la información de los candidatos en el sistema  
- **Para:** Centralizar y optimizar el proceso de selección, reduciendo el tiempo y errores manuales  

### ✅ Criterios de Aceptación  
- [ ] El reclutador puede agregar un nuevo candidato mediante un formulario con campos obligatorios:  
  - Nombre  
  - Correo  
  - Teléfono  
  - CV adjunto  
- [ ] El sistema debe validar y almacenar los datos correctamente en la base de datos  
- [ ] Al buscar un candidato, el sistema muestra resultados filtrados por:  
  - Nombre  
  - Habilidades  
  - Experiencia  
- [ ] El reclutador puede editar la información de un candidato y guardar los cambios  
- [ ] La IA clasifica automáticamente al candidato según sus habilidades y experiencia  

### 📝 Notas Adicionales  
- **Integración con IA:** Clasificación automática de CVs mediante algoritmos de NLP  
- **Optimización de búsqueda:** Uso de índices en la base de datos PostgreSQL para consultas rápidas  
- **Diseño Responsivo:** El formulario debe ser compatible con dispositivos móviles  

---

## 📅 User Story 2: Programación Automatizada de Entrevistas  

### 🎯 Título: Programar entrevistas automáticamente según disponibilidad  

- **Como:** Reclutador de Recursos Humanos  
- **Quiero:** Programar entrevistas automáticamente considerando la disponibilidad de candidatos y entrevistadores  
- **Para:** Agilizar la planificación y evitar conflictos de horarios  

### ✅ Criterios de Aceptación  
- [ ] El sistema permite seleccionar al candidato y al entrevistador desde una lista  
- [ ] El sistema consulta las disponibilidades y sugiere automáticamente los horarios posibles  
- [ ] El sistema envía notificaciones automáticas por:  
  - Correo (SendGrid)  
  - SMS (Twilio)  
- [ ] El reclutador puede reprogramar o cancelar la entrevista desde la interfaz  
- [ ] Las entrevistas agendadas se sincronizan automáticamente con:  
  - Google Calendar  
  - Outlook  

### 📝 Notas Adicionales  
- **Integración con servicios de notificación:**  
  - Twilio para SMS  
  - SendGrid para correos  
- **Sincronización de calendarios:**  
  - Uso de APIs para Google Calendar y Outlook  
- **Validación de conflictos:** Mediante el microservicio de programación en el backend  

---
# 📌 **Backlog de Producto para LTI ATS (Applicant Tracking System) #1**  

### 📊 **Metodología de Priorización Utilizada:** **MoSCoW (Must, Should, Could, Won’t)**  
La metodología **MoSCoW** nos permite clasificar las funcionalidades según su importancia para el lanzamiento del producto y su valor para el usuario. Esta técnica es ideal para organizar nuestro backlog de producto porque diferencia claramente lo que es **esencial (Must Have)** de lo que **puede esperar (Could/Won't Have)**.

### **Criterios de Priorización:**  
- **Must Have (M):** Funcionalidades críticas, sin ellas el sistema no cumple su objetivo principal.  
- **Should Have (S):** Importantes pero no críticas; pueden implementarse después del lanzamiento inicial.  
- **Could Have (C):** Deseables; aportan valor adicional, pero no son urgentes.  
- **Won’t Have (W):** Fuera del alcance actual, pero consideradas para futuras versiones.

---

## 📝 **Backlog de Producto - LTI ATS**  

| Prioridad              | ID  | Título                             | Descripción Breve                                                                                                                                          |
|------------------------|-----|------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Must Have (M)**       | 1   | Gestión de Candidatos              | Agregar, actualizar, buscar y gestionar candidatos, con clasificación automática mediante IA.                                                              |
| **Must Have (M)**       | 2   | Programación de Entrevistas        | Programar entrevistas automáticamente, sincronizando con calendarios y enviando notificaciones.                                                              |
| **Should Have (S)**     | 3   | Evaluación de Candidatos con IA    | Evaluar a los candidatos mediante pruebas técnicas y de personalidad, con informes detallados.                                                               |
| **Should Have (S)**     | 4   | Portal del Candidato               | Permitir que los candidatos consulten el estado de su aplicación y reciban feedback.                                                                        |
| **Could Have (C)**      | 5   | Análisis Predictivo Avanzado       | Implementar un sistema de recomendación basado en IA para predecir el éxito de un candidato.                                                                |
| **Could Have (C)**      | 6   | Integraciones con Redes Sociales   | Publicar automáticamente vacantes en LinkedIn y otras plataformas.                                                                                         |
| **Won’t Have (W)**      | 7   | Videoentrevistas Integradas        | Realizar entrevistas directamente desde la plataforma. (Pospuesto para una versión futura)                                                                 |

---

## 🧠 **Justificación de la Priorización:**  
- **Must Have (M):** Son esenciales para cumplir la promesa principal del sistema: gestión eficiente de candidatos y entrevistas. Estas funcionalidades permiten que el sistema sea funcional desde el primer día.  
- **Should Have (S):** Aportan un gran valor al proceso de selección y mejoran la experiencia del candidato, pero no son críticas para el lanzamiento inicial.  
- **Could Have (C):** Son funcionalidades que enriquecen el sistema, pero no afectan la operación básica.  
- **Won’t Have (W):** Funcionalidades interesantes, pero no esenciales para esta versión.  

---

## 🗂️ **Próximos Pasos:**  
- Refinar las **User Stories** más prioritarias (**M y S**) agregando **tareas técnicas**.  
- Planificar los primeros **Sprints** comenzando con los elementos **Must Have (M)**.  
- Definir una estrategia de pruebas (unitarias, de integración y de aceptación).  

---
# **Backlog de Producto para LTI ATS #2**  

### 1. Historias de Usuario y Prioridades  
A partir de la documentación revisada, se han identificado las siguientes historias de usuario y se han ordenado según su prioridad, considerando el impacto en el valor del producto y la viabilidad técnica:

#### **Alta Prioridad (Impulsan la Propuesta de Valor Principal)**  
- **HU1:** Como reclutador, quiero poder agregar y buscar candidatos rápidamente mediante búsqueda inteligente para reducir el tiempo de selección.  
- **HU2:** Como reclutador, quiero programar entrevistas automáticamente, sincronizando calendarios, para optimizar el proceso.  
- **HU3:** Como reclutador, quiero evaluar candidatos mediante IA para seleccionar los mejores perfiles con base en datos.  

#### **Media Prioridad (Mejoran la Experiencia y Eficiencia)**  
- **HU4:** Como candidato, quiero tener un portal para seguir mi proceso de aplicación y recibir feedback.  
- **HU5:** Como administrador, quiero generar informes detallados sobre el proceso de reclutamiento para analizar resultados.  
- **HU6:** Como reclutador, quiero recibir notificaciones automáticas para recordar entrevistas y actualizaciones.  

#### **Baja Prioridad (Complementan y Amplían la Funcionalidad)**  
- **HU7:** Como reclutador, quiero integrar la publicación de vacantes con LinkedIn y otras plataformas.  
- **HU8:** Como administrador, quiero gestionar permisos y roles para garantizar la seguridad.  
- **HU9:** Como administrador, quiero ver un registro de actividades para auditorías.  

---

### 2. Enfoque para Determinar el Orden de Prioridades  
Se utilizó el enfoque **MoSCoW (Must have, Should have, Could have, Won't have)** combinado con una matriz de impacto vs. esfuerzo. Las historias de mayor impacto y menor complejidad se priorizaron primero.

- **HU1, HU2, HU3:** Must have, impactan directamente en la propuesta de valor del sistema.  
- **HU4, HU5, HU6:** Should have, mejoran la experiencia y la eficiencia.  
- **HU7, HU8, HU9:** Could have, complementan la funcionalidad y aportan valor adicional.  
---
- Se eligió el prompt #1 debido a que es mucho más descriptivo, específico y lleva un mejor orden, pues brinda primero el contexto del enfoque y después muestra sus resultados. 
---
# 🗂️ **Tickets de Trabajo: Gestión de Candidatos**  

---

### 📌 **1. Crear API para Gestión de Candidatos (Backend)**  
**Descripción Técnica:**  
- Desarrollar endpoints RESTful (`POST`, `PUT`, `GET`, `DELETE`) usando **Node.js con Express** para:  
  - Crear un candidato.  
  - Actualizar la información del candidato.  
  - Buscar candidatos filtrando por nombre, habilidades y experiencia.  
  - Eliminar candidatos.  
- Implementar validaciones en las solicitudes.  
- Conectar con la base de datos **PostgreSQL** mediante **Sequelize**.  

**Criterios de Aceptación:**  
- [ ] API funcional con las 4 operaciones CRUD.  
- [ ] Validaciones de campos requeridos (nombre, email, CV).  
- [ ] Búsqueda de candidatos optimizada con índices.  
- [ ] Respuestas en formato JSON.  

**Dependencias:** Configuración de la base de datos.  

**Estimación:** 8 puntos (Alta complejidad, múltiples endpoints y validaciones)  

---

### 📌 **2. Diseñar e Implementar la Base de Datos (Modelo de Candidatos)**  
**Descripción Técnica:**  
- Crear la tabla `Candidatos` en **PostgreSQL** con los siguientes campos:  
  - `id` (PK)  
  - `nombre`  
  - `email` (único)  
  - `telefono`  
  - `habilidades` (array o jsonb)  
  - `experiencia` (años)  
  - `cv_url` (URL del CV)  
  - `created_at`, `updated_at`  
- Implementar índices para búsquedas rápidas (`email`, `habilidades`).  
- Crear migraciones usando **Sequelize**.  

**Criterios de Aceptación:**  
- [ ] Migración ejecutada correctamente.  
- [ ] Índices creados para optimizar búsquedas.  
- [ ] Validación de unicidad del email.  

**Dependencias:** Ninguna.  

**Estimación:** 5 puntos (Complejidad moderada)  

---

### 📌 **3. Implementar Clasificación Automática de CVs con IA (Backend)**  
**Descripción Técnica:**  
- Desarrollar un servicio de IA en **Python (Flask)** para:  
  - Analizar el contenido del CV usando **NLP (spaCy o TensorFlow)**.  
  - Extraer habilidades y experiencia.  
  - Calcular un puntaje de compatibilidad según el perfil solicitado.  
- Conectar este servicio con el backend a través de una llamada **HTTP (API interna)**.  

**Criterios de Aceptación:**  
- [ ] Servicio funcional que recibe un CV y devuelve habilidades y puntaje.  
- [ ] Integración completa con el backend.  
- [ ] Pruebas unitarias del servicio IA.  

**Dependencias:** API de Gestión de Candidatos.  

**Estimación:** 8 puntos (Alta complejidad, integración con IA)  

---

### 📌 **4. Crear Interfaz de Gestión de Candidatos (Frontend)**  
**Descripción Técnica:**  
- Desarrollar una interfaz en **React.js** para que los reclutadores puedan:  
  - Ver una lista de candidatos (tabla paginada).  
  - Agregar un nuevo candidato mediante un formulario.  
  - Buscar candidatos por nombre, habilidades y experiencia.  
  - Editar la información de un candidato.  
- Conectar la interfaz al backend mediante **fetch/axios**.  

**Criterios de Aceptación:**  
- [ ] Lista de candidatos paginada.  
- [ ] Formulario funcional para agregar y editar.  
- [ ] Búsqueda en tiempo real.  
- [ ] Diseño responsive.  

**Dependencias:** API de Gestión de Candidatos.  

**Estimación:** 8 puntos (Alta complejidad, múltiples componentes)  

---

### 📌 **5. Implementar Autenticación y Control de Acceso (Backend + Frontend)**  
**Descripción Técnica:**  
- Añadir autenticación mediante **JWT (JSON Web Tokens)** en el backend.  
- Crear middleware para proteger los endpoints de gestión de candidatos.  
- Agregar al frontend una página de **login** y proteger rutas mediante **React Router**.  

**Criterios de Aceptación:**  
- [ ] Los endpoints están protegidos mediante JWT.  
- [ ] El sistema rechaza accesos no autenticados.  
- [ ] El frontend solicita login para acceder a la gestión de candidatos.  

**Dependencias:** API de Gestión de Candidatos, Interfaz de Gestión de Candidatos.  

**Estimación:** 5 puntos (Complejidad moderada)  

---

### 📌 **6. Pruebas Integrales de la Gestión de Candidatos**  
**Descripción Técnica:**  
- Implementar **pruebas unitarias y de integración**:  
  - Backend: Pruebas con **Jest** para los endpoints.  
  - Frontend: Pruebas de componentes con **React Testing Library**.  
- Desarrollar pruebas de extremo a extremo (E2E) con **Cypress**.  

**Criterios de Aceptación:**  
- [ ] Cobertura de pruebas superior al 80%.  
- [ ] Pruebas E2E exitosas para el flujo completo (CRUD candidatos).  

**Dependencias:** Todos los componentes (API, Base de datos, Frontend).  

**Estimación:** 5 puntos (Complejidad moderada)  

---

## 🗓️ **Resumen de Tickets y Estimaciones:**  

| Ticket | Descripción | Puntos |
|--------|-------------|---------------------|
| 1 | Crear API para Gestión de Candidatos | 8 |
| 2 | Diseñar e Implementar la Base de Datos | 5 |
| 3 | Implementar Clasificación Automática de CVs con IA | 8 |
| 4 | Crear Interfaz de Gestión de Candidatos | 8 |
| 5 | Implementar Autenticación y Control de Acceso | 5 |
| 6 | Pruebas Integrales de la Gestión de Candidatos | 5 |
| **Total:** | | **39 puntos** |

---

### 🚀 **Planificación Recomendada:**  
- **Sprint 1 (2 semanas):**  
  - Ticket 2 (BD)  
  - Ticket 1 (API CRUD)  
  - Ticket 5 (Autenticación)  

- **Sprint 2 (2 semanas):**  
  - Ticket 4 (Frontend)  
  - Ticket 3 (IA para CVs)  
  - Ticket 6 (Pruebas)  

---
