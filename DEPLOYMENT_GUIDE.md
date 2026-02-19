# Guía de Implementación - PSiCO-IUS Landing Page

## 📋 Checklist de Configuración

### 1. Configurar Formspree (Formulario de Contacto)

1. Regístrate en [Formspree.io](https://formspree.io) (gratis para hasta 50 envíos/mes)
2. Crea un nuevo formulario
3. Copia tu endpoint único (se verá como: `https://formspree.io/f/xyzabc123`)
4. En `index.html`, busca la línea 403:
   ```html
   <form action="https://formspree.io/f/TU_ENDPOINT" method="POST" id="contactForm">
   ```
5. Reemplaza `TU_ENDPOINT` con tu código real
6. En el panel de Formspree, configura:
   - **Redirection URL**: `gracias.html` (para redirigir después del envío)
   - **Email notifications**: moguelcnsef@gmail.com

### 2. Publicar en Hosting Gratuito

#### Opción A: GitHub Pages (Recomendado)

1. Los archivos ya están en el repositorio
2. Ve a **Settings** > **Pages**
3. En **Source**, selecciona la rama que contiene los archivos
4. Selecciona carpeta **/ (root)**
5. Click en **Save**
6. Tu sitio estará disponible en: `https://joelmoguel.github.io/Psico-Ius/`

#### Opción B: Netlify

1. Ve a [netlify.com](https://www.netlify.com/)
2. Arrastra los archivos `index.html` y `gracias.html` a la zona de drop
3. Netlify desplegará automáticamente
4. Puedes personalizar el dominio en la configuración

### 3. Compartir en Redes Sociales

⚠️ **IMPORTANTE**: 
- **NO** puedes insertar esta página directamente en Facebook/Instagram
- Debes publicarla en hosting externo primero
- Luego comparte el enlace público en tus posts

**Para mejores resultados en redes sociales:**
1. Comparte el URL completo de tu página
2. Facebook/Instagram generarán automáticamente una preview con:
   - Título: "PSiCO-IUS | Neurojusticia y Resiliencia Procesal"
   - Descripción del laboratorio
   - Imagen (necesitas agregar `og-image.jpg` en el servidor)

### 4. Personalización Adicional (Opcional)

#### Agregar imagen Open Graph
1. Crea una imagen 1200x630 px con el logo PSiCO-IUS
2. Súbela al hosting como `og-image.jpg`
3. Las redes sociales la usarán automáticamente en las previews

#### Cambiar colores
En `index.html`, busca las variables CSS (líneas 83-91):
```css
:root {
    --azul-profundo: #0b2447;
    --azul-medio: #1e3a8a;
    --dorado-sutil: #d4af37;
    /* etc. */
}
```

### 5. Verificación de Funcionalidad

Antes de publicar, verifica:
- ✅ El formulario envía datos correctamente
- ✅ La redirección a `gracias.html` funciona
- ✅ El botón de WhatsApp abre la conversación
- ✅ Los enlaces de email funcionan
- ✅ La página es responsive en móvil
- ✅ El smooth scroll funciona en los botones CTA

### 6. Monitoreo

**Formspree Dashboard** te mostrará:
- Número de formularios recibidos
- Datos de contacto
- Tasa de éxito/error

**WhatsApp Business** (recomendado para seguimiento profesional):
- Descarga WhatsApp Business
- Configura respuestas automáticas
- Organiza conversaciones por etiquetas

## 🔒 Consideraciones de Privacidad

- ✅ No uses Google Analytics sin consentimiento
- ✅ Formspree cumple con LGPD/GDPR
- ✅ Los datos solo se envían a moguelcnsef@gmail.com
- ✅ No hay cookies de terceros
- ✅ No hay tracking scripts

## 📱 Datos de Contacto Configurados

- **Email**: moguelcnsef@gmail.com
- **WhatsApp**: +52 56 31 03 75 75
- **Fundadores**: 
  - Psic. Joel Moguel Mondragón
  - Dr. Víctor Moreno Sánchez

## 🎨 Características Técnicas

- **Tamaño total**: ~53KB (ultra ligero)
- **Sin dependencias externas**: No jQuery, no Bootstrap
- **Compatible con**: Chrome, Firefox, Safari, Edge
- **Responsive**: Optimizado para móvil (90% del tráfico)
- **Accesibilidad**: WCAG AA compliant

## ❓ Preguntas Frecuentes

**P: ¿Puedo editar el texto?**
R: Sí, todo el texto está en HTML puro. Busca y edita directamente.

**P: ¿Cómo cambio el número de WhatsApp?**
R: Busca `525631037575` en ambos archivos y reemplaza con tu número (incluye código de país).

**P: ¿Necesito saber programar?**
R: No para uso básico. Solo para personalizaciones avanzadas.

**P: ¿Funciona en WordPress?**
R: No directamente. Esta es una página standalone. Para WordPress necesitarías convertirla a tema.

## 🚀 Próximos Pasos Recomendados

1. Configurar Formspree (5 minutos)
2. Publicar en GitHub Pages o Netlify (10 minutos)
3. Probar el formulario (2 minutos)
4. Compartir en redes sociales
5. Monitorear primeros contactos
6. Ajustar contenido según feedback

---

**Soporte**: Si necesitas ayuda, contacta al desarrollador o consulta la documentación de Formspree/GitHub Pages.
