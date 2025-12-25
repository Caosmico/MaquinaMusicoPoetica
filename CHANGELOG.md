# Changelog

Todos los cambios notables en **La Máquina Musicopoética** serán documentados en este archivo.

El formato está basado en [Keep a Changelog](https://keepachangelog.com/es-ES/1.0.0/),
y este proyecto adhiere a [Semantic Versioning](https://semver.org/lang/es/).

## [1.0.0] - 2024-12-24

### ✨ Lanzamiento Inicial

#### Agregado
- Sistema de catalogación completo de vinilos (`vinyl-collection-complete.html`)
- Formulario de 4 pasos para recolección de datos
- 21 Pathosformeln Musicales predefinidos
- Almacenamiento en LocalStorage
- Sistema de búsqueda y filtrado
- Exportación/Importación de colecciones en JSON
- Visualizador de línea de tiempo (`vinyl-timeline-visualizer.html`)
- Vista cronológica interactiva (1950-2024)
- Organización por décadas
- Filtros por Pathosformel
- Estadísticas visuales por década
- Navegación integrada entre componentes
- Documentación completa (README.md)
- Licencia MIT

#### Características Técnicas
- React 18 via CDN
- Tailwind CSS via CDN
- Sin dependencias de backend
- Totalmente funcional en modo offline (después de primera carga)
- Diseño responsive (mobile, tablet, desktop)

#### Pathosformeln Musicales Incluidos
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

### 🎯 Funcionalidades Principales

#### Vinyl Collection Database
- CRUD completo de vinilos
- Upload de imágenes por URL
- Campos: Título, Artista, Año, Sello, Estilo, Tracks interesantes
- Selección de Pathosformel con opción personalizada
- Vista previa antes de guardar
- Edición en línea
- Eliminación con confirmación

#### Timeline Visualizer
- Visualización cronológica
- Agrupación por décadas
- Tarjetas de vinilo con portada
- Modal de vista detallada
- Estadísticas por década
- Filtrado dinámico

### 🎨 Diseño
- Paleta de colores purple-pink-cyan
- Glassmorphism en elementos UI
- Gradientes animados
- Transiciones suaves
- Iconografía consistente

---

## [Unreleased] - Próximas Versiones

### Planeado para v1.1.0
- [ ] Backend con API REST
- [ ] Base de datos persistente
- [ ] Autenticación de usuarios
- [ ] Compartir colecciones públicas

### Planeado para v1.2.0
- [ ] Integración con Discogs API
- [ ] Importación automática de datos
- [ ] Modo oscuro/claro
- [ ] Temas personalizables

### Planeado para v2.0.0
- [ ] App móvil (React Native)
- [ ] Análisis de tendencias
- [ ] Gráficos interactivos
- [ ] Exportación a PDF
- [ ] Sistema de etiquetas

---

## Notas de Versión

### Inspiración
Basado en la metodología **Pathosformel** de Aby Warburg, adaptada al contexto musical para crear un sistema único de catalogación emocional de discos de vinilo.

### Compatibilidad
- Navegadores modernos (Chrome 90+, Firefox 88+, Safari 14+, Edge 90+)
- Responsive design (320px - 4K)
- No requiere instalación
- Funciona offline después de primera carga

---

**Formato del changelog**: [Keep a Changelog](https://keepachangelog.com/)  
**Versionado**: [Semantic Versioning](https://semver.org/)
