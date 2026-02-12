# Guía rápida para revisar código (para principiantes)

Si estás empezando, no te preocupes: revisar código es una habilidad que se aprende con práctica.

## 1) Empieza por el contexto

Antes de leer funciones sueltas, responde estas preguntas:

- ¿Qué problema resuelve este proyecto?
- ¿Cómo se ejecuta?
- ¿Qué dependencias usa?
- ¿Qué carpetas son las más importantes?

## 2) Recorre el proyecto de afuera hacia adentro

Orden recomendado:

1. `README.md` (si existe)
2. Archivos de configuración (`package.json`, `pyproject.toml`, etc.)
3. Carpeta principal del código (`src/`, `app/`, etc.)
4. Tests

No intentes entender todo a la vez. Primero busca una visión general.

## 3) Haz una primera lectura “rápida”

En la primera pasada, solo detecta:

- Módulos principales
- Flujo general de datos
- Puntos de entrada (por ejemplo `main`, rutas HTTP, comandos CLI)

## 4) Segunda lectura: ahora sí, en detalle

Ahora revisa por bloques pequeños:

- Una función por vez
- Un archivo por vez
- Un caso de uso por vez

Preguntas útiles:

- ¿El nombre de variables y funciones describe bien lo que hacen?
- ¿Hay funciones demasiado largas?
- ¿Hay código duplicado?
- ¿Los errores se manejan correctamente?
- ¿La lógica de negocio está separada de la parte visual o de infraestructura?

## 5) Usa una checklist simple

Checklist para revisar mejor:

- [ ] **Correctitud**: ¿Hace lo que promete?
- [ ] **Legibilidad**: ¿Se entiende fácil?
- [ ] **Mantenibilidad**: ¿Será fácil modificarlo después?
- [ ] **Seguridad**: ¿Hay validación de entradas?
- [ ] **Pruebas**: ¿Hay tests para casos normales y bordes?

## 6) Corre el proyecto y experimenta

Aprendes mucho más si ejecutas el código:

- Corre los tests
- Prueba flujos reales
- Cambia algo pequeño y observa el resultado

## 7) Cómo comentar en una revisión (estilo útil y respetuoso)

Cuando dejes feedback, intenta este formato:

- **Observación**: “Veo que esta función hace X y Y.”
- **Riesgo**: “Podría causar Z cuando la entrada sea nula.”
- **Sugerencia**: “¿Te parece separar Y en otra función?”

Evita comentarios vagos como “esto está mal” sin explicar por qué.

## 8) Mini plan de práctica (7 días)

- Día 1–2: solo estructura del proyecto
- Día 3–4: seguir un flujo de principio a fin
- Día 5: revisar 1 archivo a fondo
- Día 6: escribir comentarios de mejora
- Día 7: comparar tu revisión con la de otra persona

## 9) Comandos útiles para empezar (terminal)

- Ver estado de cambios: `git status`
- Ver historial resumido: `git log --oneline --decorate --graph -n 10`
- Ver cambios en un archivo: `git diff <archivo>`
- Buscar texto rápido: `rg "texto"`

---

Si quieres, en el siguiente paso puedo ayudarte a hacer una **revisión guiada en este repo**, archivo por archivo, como si fuera una mentoría.
