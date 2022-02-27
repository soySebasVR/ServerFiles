# Docker Papermerge

<p align="center">
    <a href="https://www.papermerge.com/">
        <img src="https://github.com/ciur/papermerge/raw/master/artwork/logo.png" width="150" alt="Pi-hole">
    </a>
</p>

Papermerge is an open source document management system (DMS).

## Template

Title: papermerge

Description: document management system

Icon URL:
https://github.com/ciur/papermerge/raw/master/artwork/logo.png
<img src="https://github.com/ciur/papermerge/raw/master/artwork/logo.png" width="30" height="30" alt="Pi-hole">

Platform: Linux

Type: Standalone

## Variables de entorno importantes
Al crear el stack

```env
TZ=America/Lima
VOL_CONFIG=
VOL_DATA=
```

- **TZ**: Timezone
- **VOL_CONFIG**: Carpeta donde se guardará configuración de pihole
- **VOL_DATA**: Carpeta donde se guardarán los documentos
