# 🎵 La Máquina Musicopoética

Sistema de catalogación de vinilos inspirado en la metodología **Pathosformel** de Aby Warburg, adaptado al contexto musical para identificar y mapear fórmulas emocionales en álbumes de vinilo.

## 📖 Descripción

**La Máquina Musicopoética** es una aplicación web que permite documentar, catalogar y visualizar colecciones de discos de vinilo mediante el concepto warburguiano de **Pathosformel Musical** - fórmulas emocionales y expresivas que definen la esencia de cada álbum.

### Conceptos Warburguianos Aplicados

- **Pathosformel Musical**: Fórmulas del pathos adaptadas al contexto musical
- **Nachleben** (Supervivencia): Cómo las emociones y estilos musicales persisten y se transforman a través del tiempo
- **Wanderung** (Migración): Rastreo de influencias emocionales entre diferentes épocas y estilos musicales

## 🚀 Componentes del Sistema

### 1. **Vinyl Collection Database** (`vinyl-collection-complete.html`)
Sistema principal de catalogación con proceso de 4 pasos:

#### Características:
- ✅ Almacenamiento en LocalStorage (sin backend)
- ✅ Formulario de 4 pasos para recolección de datos
- ✅ 21 Pathosformeln Musicales predefinidos
- ✅ Sistema de búsqueda y filtrado
- ✅ Exportación/Importación de colecciones (JSON)
- ✅ Edición y eliminación de registros

#### Proceso de Catalogación:
1. **Paso 1**: Imagen de portada (URL o upload)
2. **Paso 2**: Datos básicos (Título, Artista, Año, Sello, Estilo)
3. **Paso 3**: Selección de Pathosformel Musical
4. **Paso 4**: Revisión y confirmación

### 2. **Timeline Visualizer** (`vinyl-timeline-visualizer.html`)
Visualización cronológica interactiva de la colección:

#### Características:
- 📅 Línea de tiempo cronológica (1950-2024)
- 🎨 Vista de cuadrícula organizada por décadas
- 🔍 Filtros por Pathosformel
- 📊 Estadísticas visuales por década
- 🎯 Vista detallada de cada vinilo

## 🎭 Pathosformeln Musicales (21 categorías)

1. Melancolía introspectiva
2. Éxtasis festivo
3. Rebeldía punk
4. Nostalgia romántica
5. Furia desenfrenada
6. Serenidad contemplativa
7. Euforia psicodélica
8. Angustia existencial
9. Triunfo épico
10. Intimidad confesional
11. Desenfreno dionisíaco
12. Desolación post-industrial
13. Misticismo espiritual
14. Ironía postmoderna
15. Resistencia política
16. Hedonismo decadente
17. Pureza minimalista
18. Caos experimental
19. Lamento blues
20. Vitalidad afrobeat
21. Otro (especificar)

## 📁 Estructura del Proyecto

```
la-maquina-musicopoetica/
│
├── README.md                           # Este archivo
├── vinyl-collection-complete.html      # Sistema de catalogación principal
├── vinyl-timeline-visualizer.html      # Visualizador de línea de tiempo
└── LICENSE                             # Licencia MIT
```

## 🛠️ Tecnologías

- **Frontend**: React 18 (via CDN)
- **Estilos**: Tailwind CSS (via CDN)
- **Almacenamiento**: LocalStorage API
- **Formato de datos**: JSON

## 🚀 Instalación y Uso

### Opción 1: Uso Directo (Sin instalación)

1. Descarga los archivos HTML
2. Abre `vinyl-collection-complete.html` en tu navegador
3. ¡Comienza a catalogar!

### Opción 2: Servidor Local

```bash
# Opción con Python
python -m http.server 8000

# Opción con Node.js
npx http-server

# Luego abre: http://localhost:8000/vinyl-collection-complete.html
```

## 📊 Modelo de Datos

### Estructura de un Vinilo

```javascript
{
  id: "1234567890",
  imageUrl: "https://example.com/cover.jpg",
  title: "Dark Side of the Moon",
  artist: "Pink Floyd",
  year: "1973",
  label: "Harvest Records",
  style: "Progressive Rock",
  interestingTracks: "Time, Money, Us and Them",
  pathosformel: "Melancolía introspectiva",
  createdAt: "2024-12-24T10:30:00.000Z"
}
```

## 🎯 Funcionalidades Principales

### Sistema de Catalogación
- ✅ Agregar nuevos vinilos
- ✅ Editar registros existentes
- ✅ Eliminar vinilos
- ✅ Búsqueda por título, artista o estilo
- ✅ Filtrado por Pathosformel
- ✅ Vista previa de portadas

### Visualización
- 📅 Línea de tiempo interactiva
- 🎨 Organización por décadas
- 📊 Estadísticas por período
- 🔍 Vista detallada de cada álbum

### Gestión de Datos
- 💾 Exportar colección (JSON)
- 📥 Importar colección (JSON)
- 🔄 Sincronización con LocalStorage

## 🎨 Paleta de Colores

### Tema Principal
- Fondo: Gradiente `slate-900 → purple-900 → slate-900`
- Acentos: `purple-500`, `pink-500`, `cyan-500`
- Textos: `white`, `purple-200`, `gray-900`

### Pathosformeln (colores por categoría)
- Melancolía: `blue-500`
- Éxtasis: `pink-500`
- Rebeldía: `red-600`
- Nostalgia: `amber-500`
- Y más...

## 🔄 Navegación entre Componentes

Desde la vista principal de **Vinyl Collection Database**:
- **Añadir Vinilo** → Formulario de catalogación
- **Mi Colección** → Vista de grid con búsqueda
- **Timeline Visualizer** → Abre visualizador en nueva pestaña

## 📈 Futuras Mejoras

- [ ] Backend con API REST
- [ ] Base de datos persistente (MongoDB/PostgreSQL)
- [ ] Autenticación de usuarios
- [ ] Compartir colecciones
- [ ] Integración con Discogs API
- [ ] Modo oscuro/claro
- [ ] App móvil (React Native)
- [ ] Análisis de tendencias emocionales
- [ ] Exportación a PDF
- [ ] Sistema de etiquetas personalizadas

## 🤝 Inspiración y Referencias

### Aby Warburg (1866-1929)
Historiador del arte alemán, creador del concepto **Pathosformel** y del **Atlas Mnemosyne**.

**Conceptos clave aplicados:**
- **Pathosformel**: Gestos y expresiones emocionales que sobreviven en el arte
- **Nachleben der Antike**: Supervivencia de elementos culturales
- **Bilderatlas**: Atlas de imágenes para mapear conexiones visuales

### Adaptación Musical
Este proyecto adapta la metodología warburguiana al contexto musical, identificando "fórmulas emocionales" en álbumes de vinilo y rastreando su supervivencia y transformación a través de décadas musicales.

## 📄 Licencia

MIT License - Libre para uso personal y comercial

## 👤 Autor

**Proyecto: La Máquina Musicopoética**  
Inspirado en la metodología de Aby Warburg  
Diciembre 2024

## 🌟 Agradecimientos

- Aby Warburg por el concepto de Pathosformel
- La comunidad de coleccionistas de vinilo
- Los creadores de React y Tailwind CSS

---

**Nota**: Este es un proyecto experimental que combina historia del arte, musicología y tecnología web para crear una herramienta única de catalogación emocional de música.

🎵 *"La música es la memoria emocional de la humanidad"* 🎵
