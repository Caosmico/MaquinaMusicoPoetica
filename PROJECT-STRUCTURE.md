# 📁 Estructura del Proyecto

```
la-maquina-musicopoetica/
│
├── 📄 README.md                          # Documentación principal del proyecto
│   ├── Descripción general
│   ├── Conceptos Warburguianos
│   ├── Componentes del sistema
│   ├── 21 Pathosformeln Musicales
│   ├── Modelo de datos
│   ├── Tecnologías
│   └── Roadmap de futuras mejoras
│
├── 🚀 QUICKSTART.md                      # Guía de inicio rápido
│   ├── Instalación en 3 pasos
│   ├── Primera catalogación (ejemplo)
│   ├── Tips y trucos
│   ├── Resolución de problemas
│   └── FAQ
│
├── 📋 CHANGELOG.md                       # Historial de versiones
│   ├── v1.0.0 - Lanzamiento inicial
│   ├── Features implementadas
│   └── Versiones planeadas
│
├── 🤝 CONTRIBUTING.md                    # Guía de contribución
│   ├── Código de conducta
│   ├── Cómo reportar bugs
│   ├── Cómo sugerir mejoras
│   ├── Pull request process
│   ├── Guías de estilo
│   └── Agregar nuevos Pathosformeln
│
├── ⚖️  LICENSE                           # Licencia MIT
│
├── 🙈 .gitignore                         # Archivos ignorados por Git
│
├── 💿 vinyl-collection-complete.html     # ★ APLICACIÓN PRINCIPAL ★
│   │
│   ├── 🏠 Vista Home
│   │   ├── Header con navegación
│   │   ├── Hero section
│   │   ├── 3 botones principales:
│   │   │   ├── Añadir Vinilo
│   │   │   ├── Mi Colección
│   │   │   └── Timeline Visualizer
│   │   └── Estadísticas (4 métricas)
│   │
│   ├── ➕ Vista Agregar/Editar
│   │   ├── Paso 1: Imagen de portada
│   │   │   ├── Opción: URL
│   │   │   └── Opción: Upload
│   │   ├── Paso 2: Datos básicos
│   │   │   ├── Título*
│   │   │   ├── Artista*
│   │   │   ├── Año
│   │   │   ├── Sello discográfico
│   │   │   ├── Estilo
│   │   │   └── Tracks interesantes
│   │   ├── Paso 3: Pathosformel
│   │   │   ├── 21 opciones predefinidas
│   │   │   └── Opción personalizada
│   │   └── Paso 4: Revisión
│   │       ├── Vista previa completa
│   │       ├── Edición rápida
│   │       └── Confirmar/Publicar
│   │
│   ├── 📚 Vista Colección
│   │   ├── Header con búsqueda
│   │   ├── Filtros:
│   │   │   ├── Búsqueda por texto
│   │   │   └── Filtro por Pathosformel
│   │   ├── Grid de vinilos
│   │   │   ├── Imagen de portada
│   │   │   ├── Título y artista
│   │   │   ├── Año y estilo
│   │   │   ├── Tag de Pathosformel
│   │   │   └── Botones: Editar/Eliminar
│   │   └── Paginación
│   │
│   ├── 💾 DataService (LocalStorage)
│   │   ├── getAll()
│   │   ├── create()
│   │   ├── update()
│   │   ├── delete()
│   │   ├── getById()
│   │   ├── exportCollection()
│   │   └── importCollection()
│   │
│   └── 🎨 Componentes React
│       ├── FormStep1 (Imagen)
│       ├── FormStep2 (Datos básicos)
│       ├── FormStep3 (Pathosformel)
│       ├── FormStep4 (Revisión)
│       ├── CollectionView
│       ├── ProgressIndicator
│       └── Icon components
│
└── 📅 vinyl-timeline-visualizer.html     # ★ VISUALIZADOR ★
    │
    ├── 🎯 Vista Principal
    │   ├── Header con filtros
    │   │   └── Filtro por Pathosformel
    │   │
    │   ├── Timeline Cronológico
    │   │   ├── Años 50 (1950-1959)
    │   │   ├── Años 60 (1960-1969)
    │   │   ├── Años 70 (1970-1979)
    │   │   ├── Años 80 (1980-1989)
    │   │   ├── Años 90 (1990-1999)
    │   │   ├── Años 2000 (2000-2009)
    │   │   ├── Años 2010 (2010-2019)
    │   │   └── Años 2020 (2020-2024)
    │   │
    │   ├── Cada década muestra:
    │   │   ├── Header con rango de años
    │   │   ├── Contador de vinilos
    │   │   └── Grid de tarjetas
    │   │
    │   ├── Tarjeta de vinilo:
    │   │   ├── Imagen de portada
    │   │   ├── Año destacado
    │   │   ├── Título
    │   │   ├── Artista
    │   │   ├── Tag de Pathosformel
    │   │   └── Click → Modal detallado
    │   │
    │   └── Modal de Detalles
    │       ├── Imagen grande
    │       ├── Todos los datos
    │       ├── Tag de Pathosformel
    │       └── Botón cerrar
    │
    ├── 📊 DataService (LocalStorage)
    │   ├── Lectura desde mismo storage
    │   ├── Sincronizado con Collection
    │   └── Agrupación por década
    │
    └── 🔧 Funciones
        ├── Filtrado dinámico
        ├── Agrupación por década
        ├── Ordenamiento cronológico
        └── Estadísticas por período
```

---

## 🎯 Flujo de Datos

```
┌─────────────────────────────────────────┐
│   Usuario abre aplicación               │
│   vinyl-collection-complete.html        │
└────────────────┬────────────────────────┘
                 │
                 ▼
┌─────────────────────────────────────────┐
│   LocalStorage (navegador)              │
│   ┌─────────────────────────────────┐   │
│   │  Clave: 'vinyl_collection'      │   │
│   │  Valor: [Array de objetos]      │   │
│   └─────────────────────────────────┘   │
└────────────────┬────────────────────────┘
                 │
                 ├──→ CRUD Operations
                 │    ├── Create (POST)
                 │    ├── Read (GET)
                 │    ├── Update (PUT)
                 │    └── Delete (DELETE)
                 │
                 ├──→ Export → JSON file
                 │
                 └──→ Import ← JSON file
                 
                 
┌─────────────────────────────────────────┐
│   Timeline Visualizer lee mismo         │
│   LocalStorage para visualización       │
└─────────────────────────────────────────┘
```

---

## 🗂️ Modelo de Datos

```javascript
{
  // Generado automáticamente
  id: "1703468400000",
  createdAt: "2024-12-24T10:30:00.000Z",
  
  // Datos del usuario
  imageUrl: "https://example.com/cover.jpg",
  title: "Dark Side of the Moon",
  artist: "Pink Floyd",
  year: "1973",
  label: "Harvest Records",
  style: "Progressive Rock",
  interestingTracks: "Time, Money, Us and Them",
  pathosformel: "Melancolía introspectiva"
}
```

---

## 🎨 Tecnologías Utilizadas

```
Frontend:
├── React 18.2.0          (via CDN)
├── Babel Standalone      (JSX transpiling)
└── Tailwind CSS 3.x      (via CDN)

Storage:
└── LocalStorage API      (Web API nativa)

Build:
└── Ninguno requerido     (Standalone HTML)
```

---

## 📦 Tamaño de Archivos

```
vinyl-collection-complete.html    ~70 KB
vinyl-timeline-visualizer.html    ~38 KB
README.md                         ~7.5 KB
QUICKSTART.md                     ~7.5 KB
CONTRIBUTING.md                   ~6.5 KB
CHANGELOG.md                      ~3.5 KB
LICENSE                           ~1 KB
.gitignore                        ~0.3 KB
─────────────────────────────────────────
TOTAL (sin comprimir)             ~135 KB
ZIP comprimido                    ~30 KB
```

---

## 🚀 Deployment Options

```
Option 1: GitHub Pages
├── Fork el repositorio
├── Settings → Pages
└── Deploy desde main branch

Option 2: Netlify Drop
├── Arrastra carpeta a netlify.com/drop
└── Obtienes URL instantánea

Option 3: Vercel
├── Conecta repositorio
└── Auto-deploy en cada push

Option 4: Local
├── Doble click en HTML
└── ¡Funciona inmediatamente!
```

---

## 📝 Archivos de Configuración

```
.gitignore        → Archivos ignorados por Git
LICENSE           → MIT License
README.md         → Docs principal
CHANGELOG.md      → Historial de cambios
CONTRIBUTING.md   → Guía de contribución
QUICKSTART.md     → Inicio rápido
```

---

## 🎵 21 Pathosformeln (Referencia rápida)

```
Introspectivas:        Energéticas:           Rebeldes:
├── Melancolía         ├── Éxtasis festivo    ├── Rebeldía punk
├── Angustia           ├── Euforia            ├── Furia
└── Nostalgia          └── Vitalidad          └── Resistencia

Contemplativas:        Intensas:              Especiales:
├── Serenidad          ├── Triunfo épico      ├── Intimidad
├── Pureza             ├── Desenfreno         ├── Ironía
└── Misticismo         └── Caos               └── Hedonismo

Blues/Otros:
├── Lamento blues
├── Desolación post-industrial
└── Otro (especificar)
```

---

**Última actualización**: Diciembre 2024  
**Versión**: 1.0.0  
**Proyecto**: La Máquina Musicopoética
