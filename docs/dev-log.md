# Bitácora de Desarrollo (`dev-log.md`)

Este documento describe paso a paso el proceso de construcción del proyecto de arquitectura basada en STATIC CONTENT HOSTING.

---

### Creación y configuración de recursos

Primero, se creó el storage account

![](./images/storageImpl.png)

Habilitamos la opción de Static Web Site y configuramos el índice y la ruta de acceso del error

![](./images/staticWebSiteConf.png)

### Creación y carga de archivos estáticos

Generamos los archivos estáticos para subirlos al Storage Account

![](./images/staticContent.png)

Ahora hay que subir los archivos estáticos al contenedor `web`

![](./images/loadData.png)

### Captura del funcionamiento

![](./images/loadedData.png)

![](./images/working.png)
