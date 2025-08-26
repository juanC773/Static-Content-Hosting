# Azure Static Content Hosting Pattern Demo

## Descripción

Implementación de demostración del **Static Content Hosting Pattern** utilizando Azure Blob Storage para servir contenido estático de forma optimizada, escalable y costo-eficiente.

## Objetivos del Proyecto

- Demostrar la separación de contenido estático vs dinámico
- Mostrar optimización de costos usando Storage en lugar de Compute
- Implementar escalabilidad automática para assets estáticos
- Reducir carga en servidores web principales

## Estructura del Proyecto

```
azure-static-content-demo/
├── README.md
├── docs/
│   └── dev-log.md          # Bitácora del proceso de desarrollo
└── static-files/           # Archivos estáticos para deployment
    ├── index.html          # Página principal
    └── styles.css          # Estilos CSS

```

## Configuración Implementada

### Storage Account

- **Tipo:** StorageV2 (General Purpose v2)
- **Performance:** Standard
- **Región:** East US
- **Redundancia:** LRS (Local Redundant Storage)

### Static Website Configuration

- **Index document:** `index.html`
- **Error document:** `404.html` (opcional)
- **Endpoint público:** Habilitado

## Tecnologías Utilizadas

- **Azure Blob Storage** - Almacenamiento de archivos estáticos
- **HTML5/CSS3** - Frontend básico para demostración
- **Responsive Design** - Compatible con dispositivos móviles

## URL de Demostración

El sitio está disponible en:

[`https://strgdemo0017umb74lauctje.z13.web.core.windows.net/`](https://strgdemo0017umb74lauctje.z13.web.core.windows.net/)

## Beneficios Demostrados

### Costo-Eficiencia

- Storage costs: ~$0.02 USD por GB/mes
- Sin costos de compute para contenido estático
- Pago solo por almacenamiento y transferencia

### Performance

- Servicio directo desde edge locations
- Reduced latency para usuarios globales
- Separación de concerns: estático vs dinámico

### Simplicidad

- Zero-code deployment
- Automatic HTTPS

## Casos de Uso

### 1. **Single Page Applications (SPA)**

- React, Angular, Vue.js apps
- Todo el frontend servido desde Blob Storage
- APIs dinámicas consumidas via AJAX/Fetch

### 2. **Static Assets para Apps Tradicionales**

- CSS, JS, imágenes servidas desde CDN
- Aplicación principal en App Service/VM
- Reduced server load

### 3. **Documentation Sites**

- Documentación técnica
- Blogs estáticos (Jekyll, Hugo)
- Landing pages

### Consideraciones Adicionales

- **Custom Domain:** Para branding profesional
- **CDN:** Para performance global
- **Private Endpoints:** Para acceso restringido

## Documentación Adicional

- **Process Log:** Ver [docs/dev-log.md](./docs/dev-log.md) para detalles del proceso
- **Azure Docs:** [Static Website Hosting](https://docs.microsoft.com/azure/storage/blobs/storage-blob-static-website)
- **Static Content Hosting:** [Pattern](https://learn.microsoft.com/en-us/azure/architecture/patterns/static-content-hosting)

**Autores:** [Alejandro Torres Soto](https://github.com/AlejandroTorres05) y [Juan David Calderón Salamanca](https://github.com/juanC773)
**Propósito:** Demostración Azure Static Content Hosting Pattern
