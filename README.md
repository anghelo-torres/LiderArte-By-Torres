name=README.md
# 🚀 LiderArte by Torres - Landing Page

Bienvenido a la landing page profesional de **LiderArte by Torres**, una plataforma de transformación de liderazgo para líderes emergentes.

## 📋 Descripción del Proyecto

Esta es una landing page de alto rendimiento diseñada para:
- ✅ Captar leads cualificados
- ✅ Convertir visitantes en clientes
- ✅ Presentar el programa "El Despertar de un Líder"
- ✅ Mostrar el Modelo TORRES de liderazgo práctico
- ✅ Ofrecer múltiples niveles de servicios (infoproducto, curso, programa, mentoría)

## 🎨 Características Principales

### Diseño
- **Responsive**: Funciona perfectamente en desktop, tablet y móvil
- **Moderno y elegante**: Paleta de colores (blanco, negro, azul, celeste)
- **Optimizado para conversión**: CTAs claros en toda la página
- **Carga rápida**: HTML/CSS/JS puro sin dependencias pesadas

### Secciones Incluidas

1. **Navegación Sticky** - Acceso rápido a todas las secciones
2. **Hero Section** - Promesa clara de transformación
3. **Sección de Problemas** - Pain points de líderes emergentes
4. **Modelo TORRES** - Framework proprietary explicado
5. **El Programa** - Descripción de beneficios
6. **6 Módulos** - Contenido estructurado por semanas
7. **Servicios Escalonados** - 5 opciones de inversión
8. **CTA Principal** - Llamado a la acción convertidor
9. **Footer** - Información legal y redes sociales

## 📁 Estructura de Archivos

```
liderarte-landing/
├── index.html          # Página principal
├── styles.css          # Estilos profesionales
├── script.js           # Interactividad y animaciones
├── README.md           # Este archivo
├── assets/             # Carpeta de imágenes
│   ├── logo.png        # Logo LiderArte by Torres
│   └── framework-torres.png  # Diagrama del Modelo TORRES
└── .gitignore         # Archivos a ignorar en Git
```

## 🎯 Paleta de Colores

| Color | Hex Code | Uso |
|-------|----------|-----|
| Azul Profesional | `#0052CC` | Botones, acentos, links |
| Azul Celeste | `#00B4D8` | Hover states, highlights |
| Negro Oscuro | `#1A1A1A` | Textos principales |
| Blanco | `#FFFFFF` | Fondo principal |
| Gris Neutro | `#F5F7FA` | Secciones alternas |

## 🚀 Cómo Usar

### 1. Instalación Local

```bash
# Clonar el repositorio
git clone https://github.com/anghelo-torres/liderarte-landing.git

# Navegar a la carpeta
cd liderarte-landing

# Abrir en navegador (opción 1)
open index.html  # Mac
start index.html # Windows
xdg-open index.html # Linux

# Opción 2: Usar un servidor local
python -m http.server 8000
# Luego visita http://localhost:8000
```

### 2. Personalización

#### Cambiar Colores
Edita las variables en `styles.css`:

```css
:root {
    --primary-blue: #0052CC;
    --secondary-blue: #00B4D8;
    /* ... más variables */
}
```

#### Modificar Contenido
- Edita textos en `index.html`
- Actualiza la información de servicios
- Personaliza los módulos del programa

#### Añadir Imágenes
1. Coloca tus imágenes en la carpeta `assets/`
2. Actualiza las rutas en `index.html`:

```html
<img src="assets/tu-imagen.png" alt="Descripción">
```

#### Conectar Formularios
En `script.js`, implementa la lógica para:
- Capturar formularios
- Enviar a tu servicio de email (Mailchimp, ConvertKit, etc.)
- Crear leads en tu CRM

Ejemplo con Mailchimp:
```javascript
// En script.js
function submitForm(email, nombre) {
    // Lógica para enviar a Mailchimp
}
```

## 📊 Optimización para Conversión

### SEO Básico
- ✅ Meta tags en el `<head>`
- ✅ Titles y descriptions claros
- ✅ Headings H1, H2, H3 estructurados
- ✅ URLs amigables

### Velocidad
- ✅ Sin dependencias externas innecesarias
- ✅ CSS y JS optimizados
- ✅ Imágenes comprimidas

### Conversión
- ✅ CTAs claros y múltiples
- ✅ Colores de botones contrastantes
- ✅ Propuesta de valor inmediata
- ✅ Testimonios y prueba social
- ✅ Garantía de satisfacción

## 🔗 Integración Recomendada

Para maximizar conversión, integra con:

1. **Email Marketing**
   - Mailchimp
   - ConvertKit
   - ActiveCampaign

2. **CRM**
   - HubSpot
   - Pipedrive
   - Salesforce

3. **Análisis**
   - Google Analytics 4
   - Mixpanel
   - Segment

4. **Pagos**
   - Stripe
   - Gumroad
   - Thinkific

## 📱 Testing Recomendado

- [ ] Prueba en Chrome, Firefox, Safari, Edge
- [ ] Verifica en mobile (iPhone, Android)
- [ ] Prueba todas las CTAs
- [ ] Verifica links internos
- [ ] Comprueba velocidad (PageSpeed)

## 📈 Métricas a Rastrear

1. **Tasa de conversión**: % de visitantes que se convierten
2. **Tasa de rebote**: % que se van sin interactuar
3. **Tiempo en página**: Segundos promedio en el sitio
4. **CTR**: Click-through rate en CTAs
5. **Secciones más vistas**: Qué resuena con la audiencia

## 🤝 Personalización Avanzada

### Añadir Testimonios
```html
<div class="testimonial">
    <p>"Cita del cliente"</p>
    <p><strong>- Nombre, Empresa</strong></p>
</div>
```

### Añadir Contador de Stats
```html
<div class="stat">
    <div class="stat-number">500+</div>
    <div class="stat-label">Líderes Transformados</div>
</div>
```

### Implementar Chat en Vivo
Integra Intercom, Drift o Zendesk Chat

## 🛡️ Seguridad

- [ ] HTTPS habilitado
- [ ] Validación de formularios
- [ ] Protección contra CSRF
- [ ] Rate limiting en formularios

## 📞 Soporte y Contribuciones

¿Encuentras un bug? ¿Tienes sugerencias?
- Abre un [Issue en GitHub](https://github.com/anghelo-torres/liderarte-landing/issues)
- Crea un [Pull Request](https://github.com/anghelo-torres/liderarte-landing/pulls)

## 📄 Licencia

Este proyecto es propiedad de **LiderArte by Torres**. Todos los derechos reservados.

---

**Última actualización**: Abril 2026
**Versión**: 1.0.0
**Autor**: Anghelo Torres

¡Hecho con 💙 para líderes emergentes!