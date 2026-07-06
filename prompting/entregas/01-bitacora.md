# 📓 Bitácora de Prompts — Ejercicio N° 01

---

## Datos

- **Alumno/a:** Maica y Mica
- **Ejercicio:** N° 01 — Nueva tabla y su CRUD
- **Fecha:** 06/07/2026
- **Modelo de IA usado:** Gemini

---

## 1. 🎯 Qué me pidieron

Resumí en 2–3 líneas el objetivo del ejercicio con tus palabras (no copiado del enunciado).
El objetivo de este ejercicio fue crear una nueva entidad llamada "materias" en la base de datos y desarrollar sus 5 endpoints correspondientes (CRUD completo) en el backend, emulando de forma exacta el patrón de diseño y la arquitectura en capas (Repository -> Service -> Controller) ya existente en el proyecto base.
---

## 2. 💬 Mis prompts (en orden)

### Prompt #1

**Lo que escribí:**
```text
Actúa como un desarrollador backend experto en Node.js, Express y PostgreSQL sin ORM. 

Contexto: Estoy trabajando en una API REST con arquitectura en capas (Controller -> Service -> Repository). El acceso a datos se delega en un helper personalizado llamado DbPg que expone 4 métodos: queryAll, queryOne, queryReturnId y queryRowCount. 

Tengo que crear el CRUD para una nueva tabla llamada "materias". Te adjunto como referencia exacta de estilo y arquitectura el archivo `cursos-repository.js`:
[Código de cursos-repository.js]

Tarea: Basándote estrictamente en el patrón anterior, generá ÚNICAMENTE el archivo `src/repositories/materias-repository.js` para la entidad "materias" (campos: id y nombre). 

Restricciones: 
- No uses ORMs ni librerías nuevas.
- Mantené las queries parametrizadas ($1, $2, etc.) para evitar SQL Injection.
- Utilizá exactamente las mismas convenciones de nomenclatura (métodos Async, etc.).
- No generes las capas de Service o Controller todavía; vamos paso a paso.