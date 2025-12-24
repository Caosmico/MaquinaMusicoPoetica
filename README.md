# 💿 Vinyl Collection Database

<div align="center">

![Vinyl Collection](https://img.shields.io/badge/Vinyl-Collection-purple?style=for-the-badge&logo=apple-music)
![React](https://img.shields.io/badge/React-18-blue?style=for-the-badge&logo=react)
![LocalStorage](https://img.shields.io/badge/Storage-LocalStorage-orange?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI+PHBhdGggZmlsbD0id2hpdGUiIGQ9Ik0xMiAyQzYuNDggMiAyIDYuNDggMiAxMnM0LjQ4IDEwIDEwIDEwIDEwLTQuNDggMTAtMTBTMTcuNTIgMiAxMiAyek0xMiAyMGMtNC40MSAwLTgtMy41OS04LThzMy41OS04IDgtOCA4IDMuNTkgOCA4LTMuNTkgOC04IDh6Ii8+PC9zdmc+)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

**Una aplicación de catalogación de vinilos inspirada en la metodología Pathosformel de Aby Warburg**

[Demo en Vivo](#-demo) • [Características](#-características) • [Instalación](#-instalación) • [Uso](#-uso)

---

### 🎵 Captura de Pantalla

![Vinyl Collection App](https://via.placeholder.com/800x450/1e1b4b/ffffff?text=Vinyl+Collection+Database)
*Interfaz principal de la aplicación*

</div>

---

## 📖 Sobre el Proyecto

**Vinyl Collection Database** es una aplicación web para catalogar discos de vinilo que va más allá de un simple inventario. Inspirada en la metodología del historiador de arte **Aby Warburg**, permite identificar **Pathosformeln Musicales** (fórmulas emocionales) que caracterizan cada álbum.

### 🎯 Filosofía del Proyecto

> "La música, como el arte visual, transmite emociones y gestos que sobreviven a través del tiempo"

Este proyecto adapta el concepto warburguiano de **Pathosformel** al contexto musical, permitiendo catalogar no solo datos técnicos, sino la **esencia emocional** de cada disco.

---

## ✨ Características

### 🎨 Catalogación Completa
- ✅ **Portada del álbum** - URL o subida de archivos (drag & drop)
- ✅ **Datos básicos** - Título, artista, año, sello discográfico
- ✅ **Estilo musical** - Clasificación libre (Rock, Jazz, Blues, etc.)
- ✅ **Tracks destacados** - Anota tus canciones favoritas
- ✅ **Pathosformel Musical** - 21 fórmulas emocionales predefinidas

### 🔍 Funcionalidades Avanzadas
- 🔎 **Búsqueda en tiempo real** por título, artista o estilo
- 🏷️ **Filtros** por Pathosformel
- 📊 **Estadísticas reales** de tu colección
- ✏️ **Editar** vinilos existentes
- 🗑️ **Eliminar** vinilos
- 💾 **Exportar/Importar** colección en JSON
- 📱 **Responsive** - Funciona en móvil, tablet y desktop

### 💿 Los 21 Pathosformeln Musicales

<details>
<summary>Ver lista completa de fórmulas emocionales</summary>

1. Melancolía introspectiva
2. Éxtasis festivo
3. Rebeldía punk
4. Serenidad contemplativa
5. Furia desatada
6. Nostalgia romántica
7. Angustia existencial
8. Triunfo épico
9. Sensualidad envolvente
10. Protesta social
11. Euforia psicodélica
12. Lamento blues
13. Energía frenética
14. Misticismo espiritual
15. Desencanto urbano
16. Pasión desenfrenada
17. Soledad urbana
18. Esperanza resiliente
19. Ironía sardónica
20. Éxtasis trascendental
21. Otro (especificar)

</details>

---

## 🚀 Demo

### 🌐 Demo en Vivo
> 🔗 [Prueba la aplicación aquí](#) *(Próximamente en GitHub Pages)*

### 📦 Demo Local (Sin Instalación)
Simplemente descarga y abre `vinyl-collection-complete.html` en tu navegador:

```bash
# Clonar el repositorio
git clone https://github.com/tu-usuario/vinyl-collection.git

# Abrir el archivo HTML
cd vinyl-collection
open demo/vinyl-collection-complete.html
```

¡Listo! No necesitas servidor ni instalación. 🎉

---

## 📥 Instalación

### Opción 1: Demo Standalone (Recomendado para probar)

```bash
# 1. Clonar repositorio
git clone https://github.com/tu-usuario/vinyl-collection.git

# 2. Abrir en navegador
cd vinyl-collection/demo
open vinyl-collection-complete.html
```

**No requiere:**
- ❌ Node.js
- ❌ npm install
- ❌ Compilación
- ❌ Servidor

### Opción 2: Proyecto React (Para desarrollo)

```bash
# 1. Clonar repositorio
git clone https://github.com/tu-usuario/vinyl-collection.git
cd vinyl-collection

# 2. Instalar dependencias
npm install

# 3. Ejecutar en modo desarrollo
npm start
```

**Dependencias necesarias:**
```json
{
  "dependencies": {
    "react": "^18.2.0",
    "react-dom": "^18.2.0",
    "lucide-react": "^0.263.1"
  },
  "devDependencies": {
    "tailwindcss": "^3.3.0"
  }
}
```

---

## 🎮 Uso

### 1️⃣ Añadir un Vinilo

#### Paso 1: Portada
- **Opción A:** Pega una URL de imagen
- **Opción B:** Sube un archivo (drag & drop o click)

#### Paso 2: Datos Básicos
```
Título: The Dark Side of the Moon
Artista: Pink Floyd
Año: 1973
Sello: Harvest Records
Estilo: Progressive Rock
Tracks Interesantes:
1. Time
2. Money
3. Us and Them
```

#### Paso 3: Pathosformel
Selecciona la fórmula emocional que mejor describe el álbum:
- Ejemplo: "Melancolía introspectiva"

#### Paso 4: Revisar y Guardar
Verifica toda la información y confirma.

### 2️⃣ Gestionar Colección

- **Buscar:** Escribe en la barra de búsqueda
- **Filtrar:** Selecciona un Pathosformel específico
- **Editar:** Click en el botón azul (lápiz)
- **Eliminar:** Click en el botón rojo (papelera)
- **Exportar:** Click en el botón de descarga (💾)

---

## 🗂️ Estructura del Proyecto

```
vinyl-collection/
│
├── README.md                           # Este archivo
├── LICENSE                             # Licencia MIT
│
├── demo/
│   └── vinyl-collection-complete.html  # Demo standalone
│
├── src/
│   └── VinylCollectionApp.jsx          # Componente React principal
│
├── docs/
│   └── VINYL-README.md                 # Documentación técnica
│
└── package.json                        # Dependencias (opcional)
```

---

## 💾 Almacenamiento de Datos

### LocalStorage (Implementado)

Los datos se guardan en el **LocalStorage** del navegador:

```javascript
{
  id: "1735061234567",
  imageUrl: "https://...", // o data:image/jpeg;base64,...
  title: "The Dark Side of the Moon",
  artist: "Pink Floyd",
  year: "1973",
  label: "Harvest Records",
  style: "Progressive Rock",
  interestingTracks: "1. Time\n2. Money\n3. Us and Them",
  pathosformel: "Melancolía introspectiva",
  createdAt: "2024-12-24T12:00:00.000Z"
}
```

**Ventajas:**
- ✅ Sin servidor necesario
- ✅ Funciona offline
- ✅ Datos persisten en el navegador
- ✅ Rápido y gratuito

**Limitaciones:**
- ⚠️ Máximo ~5-10 MB por dominio
- ⚠️ Solo accesible desde el mismo navegador
- ⚠️ Se borra si se limpia el navegador

### Backend (Preparado para migrar)

El código usa un servicio `DataService` que abstrae el almacenamiento. Para migrar a backend solo necesitas cambiar:

```javascript
// Ahora:
DataService.getAll() → localStorage.getItem()

// Después:
DataService.getAll() → fetch('/api/vinyls')
```

**Arquitectura preparada para:**
- 🔄 API REST
- 🗄️ MongoDB / PostgreSQL
- ☁️ Firebase / Supabase
- 🔐 Autenticación

---

## 🛠️ Tecnologías

### Frontend
- **React 18** - Biblioteca de UI
- **Tailwind CSS** - Estilos utility-first
- **Lucide React** - Iconos
- **LocalStorage API** - Persistencia de datos

### Próximamente (Backend)
- Node.js + Express
- MongoDB
- JWT Authentication

---

## 🎨 Diseño y UX

### Paleta de Colores

**Vista Home (Tema Oscuro):**
```css
Background: gradient(slate-900 → purple-900 → slate-900)
Primary: purple-500, pink-500
Text: white, purple-200
```

**Formularios (Tema Claro):**
```css
Background: slate-50
Cards: white
Accents: purple-600, pink-600
```

### Inspiración de Diseño
- 🎨 **Estilo museo** - Fichas de catalogación elegantes
- 💿 **Cultura vinilo** - Estética retro-moderna
- 📚 **Warburg Atlas** - Diseño académico pero accesible

---

## 🤝 Contribuir

¡Las contribuciones son bienvenidas! 

### Cómo Contribuir

1. **Fork** el proyecto
2. **Crea** una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. **Commit** tus cambios (`git commit -m 'Add: Amazing Feature'`)
4. **Push** a la rama (`git push origin feature/AmazingFeature`)
5. **Abre** un Pull Request

### Ideas para Contribuir

- [ ] Integración con Discogs API
- [ ] Modo oscuro completo
- [ ] Exportar a PDF
- [ ] Gráficos de estadísticas
- [ ] Backend con autenticación
- [ ] App móvil (React Native)
- [ ] Integración con Spotify

---

## 📜 Licencia

Distribuido bajo la licencia MIT. Ver `LICENSE` para más información.

```
MIT License

Copyright (c) 2024 Vinyl Collection Database

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction...
```

---

## 👨‍💻 Autor

**Tu Nombre**
- GitHub: [@tu-usuario](https://github.com/tu-usuario)
- Email: tu-email@ejemplo.com

---

## 🙏 Agradecimientos

- **Aby Warburg** - Inspiración metodológica (Atlas Mnemosyne)
- **Tailwind CSS** - Framework de estilos
- **Lucide** - Librería de iconos
- **React Team** - Por React 18

---

## 📚 Recursos Adicionales

### Sobre Aby Warburg y Pathosformel

- 📖 [Atlas Mnemosyne - Wikipedia](https://en.wikipedia.org/wiki/Mnemosyne_(art_project))
- 🎨 [Warburg Institute](https://warburg.sas.ac.uk/)
- 📝 [Pathosformel: Concepto y Aplicación](https://example.com)

### Documentación del Proyecto

- 📄 [Documentación Técnica Completa](docs/VINYL-README.md)
- 🎯 [Roadmap del Proyecto](ROADMAP.md)
- 🐛 [Reportar un Bug](https://github.com/tu-usuario/vinyl-collection/issues)

---

## 📊 Estadísticas del Proyecto

![GitHub stars](https://img.shields.io/github/stars/tu-usuario/vinyl-collection?style=social)
![GitHub forks](https://img.shields.io/github/forks/tu-usuario/vinyl-collection?style=social)
![GitHub watchers](https://img.shields.io/github/watchers/tu-usuario/vinyl-collection?style=social)

---

<div align="center">

**⭐ Si este proyecto te ha sido útil, considera darle una estrella**

Hecho con 💜 y ☕ por [Tu Nombre]

[⬆ Volver arriba](#-vinyl-collection-database)

</div>
