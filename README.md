# Máster ERCSP — Demo v2

Página interactiva de elección de itinerario formativo para el **Máster Universitario en Economía, Regulación y Competencia en los Servicios Públicos** (Universidad de Barcelona).

---

## Estructura

```
├── index.html          # Página principal (demo v2)
├── README.md           # Este archivo
└── .gitignore
```

---

## Funcionalidad

### Dos rutas de acceso
- **Ya inscrito** → Formularios con envío de datos a Airtable
- **Solo interesado** → Orientación sin envío, con botón a formulario de contacto

### Itinerarios disponibles

**Plan de estudios (Español)**
- ⚖️ Juristas — 4 especializaciones con asignación automática
- 📊 Economistas — 4 especializaciones
- 🏛️ Ingenieros y Politólogos — selección en dos bloques (10 ECTS obligadas + especialidad)

**Opción bilingüe (Español/English)**
- 📊 Economistas bilingüe — con pares de disciplinas mutuamente excluyentes
- 🏛️ Ingenieros y Politólogos bilingüe — misma lógica

### Lógica de selección
- Asignación automática de disciplinas según especialización
- Bloqueo de disciplinas al alcanzar créditos máximos
- Exclusión mutua de pares de disciplinas (bilingüe)
- Popup de confirmación con resumen completo y total de créditos ECTS

---

## Configuración de Airtable

Pulsa **Ctrl+Shift+A** en la página para abrir el panel de configuración e introducir:
- API Token de Airtable
- Base ID

Los datos se guardan en el navegador local. Para producción, usar Netlify Functions.

---

## Tecnología

- HTML5 / CSS3 / JavaScript puro (sin dependencias)
- Airtable API v0
