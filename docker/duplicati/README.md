# Docker Downloarr

<p align="center">
    <a href="https://www.duplicati.com/">
        <img src="https://github.com/linuxserver/docker-templates/raw/master/linuxserver.io/img/duplicati-icon.png" width="300" alt="duplicati">
    </a>
</p>

Duplicati works with standard protocols like FTP, SSH, WebDAV as well as popular services like Microsoft OneDrive, Amazon Cloud Drive & S3, Google Drive, box.com, Mega, hubiC and many others.

## Template

Title: duplicati

Description: Free backup software to store encrypted backups

Icon URL:
https://raw.githubusercontent.com/Servarr/Wiki/master/assets/servarr/servarr_dark_1024.png
<img src="https://github.com/linuxserver/docker-templates/raw/master/linuxserver.io/img/duplicati-icon.png" width="30" height="30" alt="duplicati">

Platform: Linux

Type: Standalone

## Variables de entorno importantes
Al crear el stack

```env
TZ=
VOL_CONFIG=
VOL_BACKUP=
VOL_SOURCE=
```

- **TZ**: Timezone
- **VOL_CONFIG**: Carpeta donde se guardará configuración de pihole
- **VOL_BACKUP**: Carpeta de backup
- **VOL_SOURCE**: Carpeta de datos para hacer backup
