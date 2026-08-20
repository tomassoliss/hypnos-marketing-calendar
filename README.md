# Hypnos · Calendario Marketing 2026–2027

Sitio interno del equipo de marketing. Muestra campañas, lanzamientos e hitos por mes. Al hacer clic en cualquier ítem se despliega el detalle completo: descripción, canales, responsable, presupuesto y checklist de tareas.

## Fuente de datos

Toda la información vive en una Google Sheet privada de Hypnos. El sitio la lee automáticamente cada vez que se carga. No hay que tocar el código para actualizar datos.

**Sheet:** [Hypnos Calendario Marketing 2026–2027](https://docs.google.com/spreadsheets/d/e/2PACX-1vSAIl0c_w4UIh6NxDB--MQ1KUYTX8DjjeYc8_kAcLO-v5F8RjrHHHdytG-5wXehM5oTivVWVQt_enWH/pub)

### Pestañas

| Pestaña | Qué contiene |
|---|---|
| `Calendario` | Una fila por campaña/hito. Nombre, mes, fechas, tipo, canales, responsable, estado. |
| `Presupuesto` | Una fila por concepto de gasto. Se cruza con Calendario por `id`. |
| `Checklist` | Una fila por tarea. Se cruza con Calendario por `id`. |

### Reglas de la Sheet

- **`tipo`** solo acepta: `Lanzamiento` / `Campaña comercial` / `Campaña de marketing` / `Hito de marca` / `Producción`
- **`estado`** solo acepta: `Sin empezar` / `En curso` / `Listo` / `Pausado`
- **`hecho`** en Checklist solo acepta: `TRUE` / `FALSE`
- El **`id`** de una campaña debe ser exactamente igual en las 3 pestañas (ej: `OCT-001`)

## Cómo activar GitHub Pages

1. Ve a **Settings → Pages** en este repositorio
2. En **Source**, selecciona `Deploy from a branch`
3. Rama: `main`, carpeta: `/ (root)`
4. Guarda — en 1-2 minutos el sitio estará en `https://[tu-org].github.io/hypnos-marketing-calendar`

## Cómo agregar un ítem nuevo

1. Abre la Google Sheet
2. En la pestaña `Calendario`, agrega una fila con un `id` nuevo (ej: `ENE27-001`)
3. Agrega las filas de presupuesto y checklist correspondientes en sus pestañas con ese mismo `id`
4. Recarga el sitio — aparece automáticamente

## Acceso al equipo

Comparte el repositorio con los colaboradores que necesites en **Settings → Collaborators**.
Para que puedan editar datos, comparte la Google Sheet directamente con su correo de Google.
