# Guía de Contribución

¡Gracias por tu interés en contribuir a **La Máquina Musicopoética**! 🎵

## 📋 Tabla de Contenidos

- [Código de Conducta](#código-de-conducta)
- [¿Cómo puedo contribuir?](#cómo-puedo-contribuir)
- [Reportar Bugs](#reportar-bugs)
- [Sugerir Mejoras](#sugerir-mejoras)
- [Pull Requests](#pull-requests)
- [Guías de Estilo](#guías-de-estilo)

## 🤝 Código de Conducta

Este proyecto adhiere a un código de conducta basado en respeto y colaboración. Al participar, te comprometes a mantener un ambiente acogedor para todos.

## 🎯 ¿Cómo puedo contribuir?

### 1. Reportar Bugs

Si encuentras un bug, por favor crea un issue con:

**Título descriptivo**
```
[BUG] La búsqueda no filtra correctamente por artista
```

**Información a incluir:**
- Descripción del problema
- Pasos para reproducir
- Comportamiento esperado
- Comportamiento actual
- Screenshots (si aplica)
- Navegador y versión
- Sistema operativo

### 2. Sugerir Mejoras

¿Tienes una idea para mejorar el proyecto?

**Formato de sugerencia:**
```
[FEATURE] Agregar exportación a CSV

**Descripción**: Permitir exportar la colección en formato CSV además de JSON

**Beneficios**: 
- Compatibilidad con Excel
- Análisis de datos más fácil
- Importación a otros sistemas

**Implementación sugerida**: [opcional]
```

### 3. Contribuir Código

#### Proceso:

1. **Fork** el repositorio
2. **Crea una rama** para tu feature:
   ```bash
   git checkout -b feature/nombre-descriptivo
   ```
3. **Haz tus cambios** siguiendo las guías de estilo
4. **Commit** con mensajes descriptivos:
   ```bash
   git commit -m "feat: agregar exportación CSV"
   ```
5. **Push** a tu fork:
   ```bash
   git push origin feature/nombre-descriptivo
   ```
6. **Abre un Pull Request**

## 🐛 Reportar Bugs

### Antes de reportar:
- [ ] Busca en issues existentes
- [ ] Verifica que estás usando la última versión
- [ ] Reproduce el bug en diferentes navegadores

### Template de Bug Report:

```markdown
## Descripción del Bug
[Descripción clara y concisa]

## Pasos para Reproducir
1. Ir a '...'
2. Click en '...'
3. Scroll hasta '...'
4. Ver error

## Comportamiento Esperado
[Qué esperabas que pasara]

## Comportamiento Actual
[Qué pasó realmente]

## Screenshots
[Si aplica]

## Entorno
- Navegador: [Chrome 120]
- OS: [Windows 11]
- Versión del proyecto: [1.0.0]

## Información Adicional
[Contexto adicional]
```

## 💡 Sugerir Mejoras

### Áreas de Mejora:

1. **Nuevos Pathosformeln**
   - Sugerir nuevas categorías emocionales
   - Proponer subcategorías

2. **Funcionalidades**
   - Integración con APIs externas
   - Nuevas visualizaciones
   - Herramientas de análisis

3. **UX/UI**
   - Mejoras de diseño
   - Optimizaciones de flujo
   - Accesibilidad

4. **Rendimiento**
   - Optimizaciones de código
   - Lazy loading
   - Caching

## 🔧 Pull Requests

### Checklist antes de enviar:

- [ ] El código sigue las guías de estilo
- [ ] Los cambios son testeados en múltiples navegadores
- [ ] La documentación está actualizada
- [ ] Los commits tienen mensajes descriptivos
- [ ] No hay conflictos con la rama main

### Template de Pull Request:

```markdown
## Tipo de cambio
- [ ] Bug fix
- [ ] Nueva feature
- [ ] Breaking change
- [ ] Documentación

## Descripción
[Descripción clara de los cambios]

## ¿Por qué este cambio?
[Motivación y contexto]

## ¿Cómo se ha probado?
- [ ] Navegador X
- [ ] Navegador Y
- [ ] Mobile
- [ ] Tablet

## Screenshots
[Si aplica]

## Checklist
- [ ] Código limpio y comentado
- [ ] Sin errores de consola
- [ ] Responsive design
- [ ] Documentación actualizada
```

## 📝 Guías de Estilo

### HTML
```html
<!-- Usar indentación de 4 espacios -->
<!-- Nombres de clase descriptivos -->
<div className="bg-white rounded-xl shadow-lg">
    <h2 className="text-2xl font-bold">Título</h2>
</div>
```

### JavaScript/React
```javascript
// Usar camelCase para variables y funciones
const handleSaveVinyl = () => {
    // Código aquí
};

// Comentarios descriptivos cuando sea necesario
// Esta función filtra vinilos por pathosformel
const filterByPathosformel = (vinyls, filter) => {
    return vinyls.filter(v => v.pathosformel === filter);
};
```

### CSS/Tailwind
```javascript
// Orden de clases Tailwind:
// 1. Layout (flex, grid)
// 2. Sizing (w-, h-)
// 3. Spacing (p-, m-)
// 4. Typography (text-, font-)
// 5. Visual (bg-, border-, shadow-)
// 6. Misc (transition-, cursor-)

className="flex w-full h-screen p-6 text-lg font-bold bg-white border rounded-lg shadow-md hover:shadow-lg transition-all"
```

### Commits

Formato: `tipo(scope): descripción`

**Tipos:**
- `feat`: Nueva feature
- `fix`: Bug fix
- `docs`: Documentación
- `style`: Formato, styling
- `refactor`: Refactorización
- `test`: Tests
- `chore`: Mantenimiento

**Ejemplos:**
```bash
feat(timeline): agregar filtro por década
fix(search): corregir búsqueda case-sensitive
docs(readme): actualizar instrucciones de instalación
style(ui): mejorar espaciado en cards
refactor(data): optimizar almacenamiento localStorage
```

## 🎨 Agregar Nuevos Pathosformeln

Si quieres agregar nuevas categorías emocionales:

1. **Investiga** si la categoría no existe
2. **Propón** nombre descriptivo en español
3. **Define** características emocionales
4. **Sugiere** ejemplos de álbumes que encajan
5. **Asigna** color representativo (opcional)

**Formato de propuesta:**
```markdown
### Pathosformel: "Desolación urbana"

**Descripción**: Sensación de alienación y soledad en contextos urbanos modernos

**Características**:
- Atmósferas frías y distantes
- Letras sobre desconexión social
- Sonidos industriales/electrónicos

**Ejemplos de álbumes**:
- Joy Division - Unknown Pleasures
- Radiohead - OK Computer
- Portishead - Dummy

**Color sugerido**: `slate-600`
```

## 🌐 Internacionalización

Actualmente el proyecto está en **español**. Si quieres contribuir con traducciones:

1. Crea carpeta `i18n/[idioma]/`
2. Traduce strings manteniendo claves originales
3. Documenta proceso de cambio de idioma

## 📚 Recursos

- [React Docs](https://react.dev/)
- [Tailwind CSS](https://tailwindcss.com/docs)
- [Aby Warburg - Wikipedia](https://es.wikipedia.org/wiki/Aby_Warburg)
- [Pathosformel Concept](https://en.wikipedia.org/wiki/Pathosformel)

## ❓ Preguntas

¿Tienes dudas? Abre un issue con el tag `question` o contacta a los maintainers.

## 🙏 Agradecimientos

Gracias por ayudar a hacer **La Máquina Musicopoética** mejor para todos. Cada contribución cuenta, sin importar su tamaño.

---

**"La música es memoria emocional, y cada contribución ayuda a preservarla"** 🎵
