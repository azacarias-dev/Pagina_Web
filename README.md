# Portfolio - Fundación Kinal

Un proyecto de rediseño y modernización de la página web de la **Fundación Kinal**, un centro educativo dedicado a la formación técnica profesional en Guatemala.

---

## 📋 Tabla de Contenidos

- [Descripción del Proyecto](#descripción-del-proyecto)
- [Razones del Rediseño](#razones-del-rediseño)
- [Estructura del Proyecto](#estructura-del-proyecto)
- [Características Principales](#características-principales)
- [Decisiones de Diseño](#decisiones-de-diseño)
- [Tecnologías Utilizadas](#tecnologías-utilizadas)
- [Guía de Instalación](#guía-de-instalación)
- [Archivos Principales](#archivos-principales)

---

## 📝 Descripción del Proyecto

Este proyecto incluye el rediseño completo de la página web de la Fundación Kinal, transformándola de un sitio básico en una **plataforma moderna, atractiva y completamente responsiva** que comunica efectivamente la misión educativa de la institución.

El rediseño mantiene la identidad de Kinal mientras mejora significativamente la experiencia del usuario en todos los dispositivos (desktop, tablet y móvil).

---

## 🎯 Razones del Rediseño

### 1. **Modernización Visual**
   - La página anterior tenía un diseño desactualizado con colores planos
   - Se implementaron **gradientes modernos, animaciones suaves y efectos visuales** que dan vida a la interfaz
   - El nuevo diseño sigue tendencias actuales del diseño web (2024-2026)

### 2. **Mejor Comunicación de la Marca**
   - Se agregó una sección dedicada a **Misión, Valor y Visión** para fortalecer la identidad institucional
   - Se incluye información sobre **por qué elegir Kinal** con 6 puntos clave
   - Se agregaron **testimonios reales de egresados** para generar confianza

### 3. **Experiencia del Usuario Mejorada**
   - Navegación clara y funcional con enlaces ancla a todas las secciones
   - Mejor jerarquía visual con títulos de secciones destacados
   - Cargas más rápidas (uso de imágenes .avif optimizadas)
   - Scroll suave y fluido en toda la página

### 4. **Responsividad Completa**
   - La página anterior no se adaptaba correctamente a dispositivos móviles
   - Ahora funciona perfectamente en:
     - **Desktop** (1024px+)
     - **Tablet** (768px - 1024px)
     - **Móvil** (480px - 768px)
   - Todos los elementos se redimensionan y reorganizan automáticamente

### 5. **Más Información Accesible**
   - Se expandió el contenido sobre los **5 programas educativos** con descripciones detalladas
   - Se agregó una sección de **Logros** con estadísticas impactantes
   - Se incluye **información completa de contacto** por departamento
   - Nueva sección de **Alianzas Estratégicas** y **Redes Sociales**

### 6. **Footer Funcional y Atractivo**
   - El anterior estaba vacío
   - Ahora contiene 4 secciones organizadas:
     - Contacto por departamento educativo
     - Ubicación con dirección completa
     - Bolsa de empleos con contacto directo
     - Enlaces a redes sociales

---

## 🎨 Decisiones de Diseño

### **Paleta de Colores Expandida**

```
🔵 Azul Primario (#0057a3)
   → Color corporativo de Kinal
   → Usado en: Headers, botones principales, enlaces

🟠 Naranja (#ff9500)
   → Color de energía y acción
   → Usado en: Botones CTA, acentos, hover effects

🟢 Verde (#2ecc71)
   → Éxito y crecimiento
   → Usado en: Elementos secundarios, iconos

🟣 Púrpura (#9b59b6)
   → Profesionalismo
   → Usado en: Detalles y acentos sutiles
```

**¿Por qué?** La paleta original era muy limitada (solo azul y gris). Una paleta expandida permite:
- Mayor flexibilidad visual
- Mejor diferenciación entre secciones
- Experiencia más moderna y atractiva
- Mejor accesibilidad con contrastes adecuados

### **Tipografía: Poppins**

Se cambió de Arial/Helvetica a **Poppins** (Google Fonts)

**¿Por qué?**
- Más moderna y legible
- Disponible en múltiples pesos (300, 400, 600, 700, 800)
- Mejor en pantallas pequeñas
- Comunica profesionalismo y modernidad

### **Estructura de Grid**

Se utilizan **CSS Grid** en lugar de Flexbox para secciones

**¿Por qué?**
- Mejor control de layouts responsivos
- Más fácil de mantener
- Permite `auto-fit` para adaptar automáticamente el número de columnas
- Mejor rendimiento en navegadores modernos

### **Animaciones y Transiciones**

Se agregaron animaciones sutiles como:
- `fadeInUp` en tarjetas
- `slideDown` en navbar
- `bounce` en iconos
- Hover effects en botones y enlaces

**¿Por qué?**
- Aumentan el engagement del usuario
- Comunican interactividad
- Mejoran la percepción de calidad
- No son obstructivas (todas <0.8s)

### **Hero Section Mejorada**

Se transformó de una sección simple a una sección visualmente impactante

**Cambios:**
- Imagen de fondo con brillo reducido (brightness: 0.6)
- Botón CTA destacado "CONOCE NUESTROS PROGRAMAS"
- Posicionamiento centrado perfecto
- Responsive en todos los dispositivos

**¿Por qué?**
- Primera impresión crítica
- Comunica profesionalismo
- Guía al usuario a la acción principal
- Atrae la atención y da contexto inmediatamente

### **Tarjetas con Overlay**

Las tarjetas de programas incluyen un overlay que aparece en hover

**¿Por qué?**
- Revela el nombre del programa sin ocupar espacio
- Efecto visual atractivo
- Interactividad clara para el usuario
- Mejor jerarquía visual

### **Footer Gradiente**

Fondo con gradiente azul en el footer

**¿Por qué?**
- Cierre visual fuerte
- Diferencia clara del contenido principal
- Comunica que es una sección importante
- Contraste adecuado para la legibilidad

---

## 📂 Estructura del Proyecto

```
Pagina_Web/
├── index.html                          # Página de inicio
├── biografia.html                      # Página de biografía
├── kinal.html                          # Página principal rediseñada
├── README.md                           # Este archivo
│
├── styles/
│   ├── variables.css                   # Variables CSS (colores, fuentes)
│   └── globals.css                     # Estilos globales
│
└── componentes/
    ├── layout/
    │   ├── Header/
    │   │   ├── Header.css              # Estilos del navbar
    │   │   └── kinal_logo.avif         # Logo de Kinal
    │   └── Footer/
    │       └── Footer.css              # Estilos del footer
    │
    └── sections/
        ├── banner/
        │   ├── Hero.css                # Estilos de sección hero y misión
        │   └── [imágenes de secciones]
        ├── information/
        │   ├── info.css                # Estilos de programas y carreras
        │   └── [imágenes de programas]
        └── Contact/
            └── Contact.css             # Estilos del footer de contacto
```

---

## ✨ Características Principales

### 1. **Navegación Inteligente**
- Links funcionales a todas las secciones
- Subrayado animado en hover
- Botón "Inicio" destacado en naranja
- Responsivo en todos los tamaños de pantalla

### 2. **Secciones Informativas**
- ✅ **Hero**: Impactante con CTA
- ✅ **Misión/Valor/Visión**: Identidad institucional
- ✅ **Programas**: 5 programas educativos con descripciones
- ✅ **Por qué elegir Kinal**: 6 razones destacadas
- ✅ **Carreras**: 5 especialidades principales
- ✅ **Logros**: Estadísticas de impacto
- ✅ **Alianzas**: Espacio para empresas asociadas
- ✅ **Testimonios**: Experiencias de egresados

### 3. **Footer Completo**
- Contacto por departamento (4 direcciones de email)
- Ubicación y dirección física
- Bolsa de empleos con contacto directo
- Redes sociales funcionales
- Logo prominente

### 4. **Diseño Responsivo**
- Mobile-first approach
- Breakpoints en 480px, 768px, 1024px
- Imágenes optimizadas (.avif)
- Flex y Grid layouts adaptativos

---

## 🛠 Tecnologías Utilizadas

| Tecnología | Propósito |
|-----------|----------|
| **HTML5** | Estructura semántica |
| **CSS3** | Estilos, animaciones, responsividad |
| **CSS Variables** | Gestión centralizada de colores y valores |
| **CSS Grid** | Layouts responsivos |
| **Flexbox** | Alineación de elementos |
| **Google Fonts** | Tipografía Poppins |
| **AVIF** | Imágenes optimizadas |

---

## 🚀 Guía de Instalación

### Requisitos
- Navegador moderno (Chrome 90+, Firefox 88+, Safari 14+, Edge 90+)
- No se requieren dependencias externas

### Pasos
1. Clona o descarga el repositorio
2. Abre `kinal.html` en tu navegador
3. ¡Listo! No requiere servidor local

### Para desarrollo local (opcional)
```bash
# Si deseas usar un servidor local
cd /ruta/al/proyecto
python -m http.server 8000
# O con Node.js
npx http-server
```

---

## 📄 Archivos Principales

### `kinal.html`
Página principal rediseñada. Contiene:
- Todas las secciones del sitio
- Estructura semántica HTML5
- Links a todos los CSS necesarios

### `styles/variables.css`
Define:
- Colores (primario, secundario, acentos)
- Valores CSS reutilizables
- Tema centralizado

### `componentes/layout/Header/Header.css`
Estilos del navbar:
- Posición fija
- Responsive design
- Animaciones

### `componentes/sections/banner/Hero.css`
Estilos de secciones principales:
- Hero
- Misión/Valor/Visión
- Animaciones

### `componentes/sections/information/info.css`
Estilos de:
- Programas educativos
- Carreras
- Logros
- Testimonios
- Razones para elegir

### `componentes/sections/Contact/Contact.css`
Estilos del footer:
- Secciones de contacto
- Redes sociales
- Información de ubicación

---

## 🎯 Objetivos Logrados

✅ Diseño moderno y atractivo
✅ Completamente responsivo
✅ Fácil de navegar
✅ Más información de valor
✅ Mejor comunicación de marca
✅ Optimizado para SEO básico
✅ Rápido y eficiente
✅ Mantenible y escalable

---

## 📚 Mejoras Futuras

- [ ] Agregar formulario de contacto funcional
- [ ] Integrar backend para testimonios dinámicos
- [ ] Agregar blog de noticias
- [ ] Implementar galería de fotos
- [ ] Añadir mapas de ubicación interactivos
- [ ] Chatbot de atención al cliente
- [ ] Sistema de inscripción online
- [ ] Integración con redes sociales

---

## 👨‍💼 Autor

Rediseño realizado como parte del Portfolio Profesional

**Fecha**: Enero 2026
**Versión**: 1.0

---

## 📞 Contacto - Fundación Kinal

| Departamento | Email |
|-------------|-------|
| Educación Continua | infocet@kinal.org.gt |
| Educación Básica | infobas@kinal.org.gt |
| Escuela Técnica | infoets@kinal.org.gt |
| Tecnología e Informática | infotic@kinal.org.gt |
| Bolsa de Empleos | empleos@kinal.edu.gt |

**📍 Ubicación**: 6 avenida 13-54 zona 7, Colonia Landívar, 01007 Ciudad de Guatemala, Guatemala, C.A.

**💬 WhatsApp**: [2216-0090](https://wa.me/50222160090)

---

## 📄 Licencia

Este proyecto es parte del portfolio educativo. Todos los derechos sobre el contenido y diseño de Fundación Kinal se mantienen con la institución.

---

**Última actualización**: 25 de enero de 2026
