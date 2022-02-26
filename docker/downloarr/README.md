# Docker Downloarr

<p align="center">
    <a href="https://wiki.servarr.com/radarr">
        <img src="https://wiki.servarr.com/assets/radarr/logos/128.png" width="100" height="100" alt="radarr">
    </a>
    <a href="https://wiki.servarr.com/sonarr">
        <img src="https://wiki.servarr.com/assets/sonarr/logos/128.png" width="100" height="100" alt="sonarr">
    </a>
    <a href="https://wiki.servarr.com/readarr">
        <img src="https://wiki.servarr.com/assets/readarr/logos/128.png" width="100" height="100" alt="readarr">
    </a>
</p>
<p align="center">
    <a href="https://wiki.servarr.com/prowlarr">
        <img src="https://wiki.servarr.com/assets/prowlarr/logos/128.png" width="100" height="100" alt="prowlarr">
    </a>
    <a href="https://transmissionbt.com/">
        <img src="https://upload.wikimedia.org/wikipedia/commons/6/6d/Transmission_icon.png" width="100" height="100" alt="Transmission_icon">
    </a>
</p>

Collectively they are referred to as "*Arr" or "*Arrs". They are designed to automatically grab, sort, organize, and monitor your Music, Movie, E-Book, or TV Show collections for Lidarr, Radarr, Readarr, and Sonarr

## Template

Title: downloarr

Description: Radarr, Readarr, Sonarr, Prowlarr and Transmission

Icon URL:
https://raw.githubusercontent.com/Servarr/Wiki/master/assets/servarr/servarr_dark_1024.png
<img src="https://raw.githubusercontent.com/Servarr/Wiki/master/assets/servarr/servarr_dark_1024.png" width="30" height="30" alt="Plex">

Platform: Linux

Type: Standalone

## Variables de entorno importantes
Al crear el stack

```env
TZ=
USER=
PASSWORD=
VOL_MEDIA=
VOL_CONFIG=
```

- **TZ**: Timezone
- **USER**: Usuario para Transmission
- **PASSWORD**: Contraseña para Transmission
- **VOL_CONFIG**: Carpeta donde se guardará configuración de pihole
- **VOL_MEDIA**: Carpeta de media
