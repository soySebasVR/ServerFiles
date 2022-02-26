# Docker Plex

![plex](http://the-gadgeteer.com/wp-content/uploads/2015/10/plex-logo-e1446990678679.png)

[Plex](https://plex.tv) organizes video, music and photos from personal media libraries and streams them to smart TVs, streaming boxes and mobile devices.

## Template

Title: plex

Description: Organizes video, music and photos

Icon URL:
https://styles.redditmedia.com/t5_2ql7e/styles/communityIcon_mdwl2x2rtzb11.png
<img src="https://styles.redditmedia.com/t5_2ql7e/styles/communityIcon_mdwl2x2rtzb11.png" width="30" height="30" alt="Plex">

Platform: Linux

Type: Standalone

## Variables de entorno importantes
Al crear el stack

```env
TZ=America/Lima
VOL_CONFIG=
VOL_MEDIA=
```

- **TZ**: Timezone
- **VOL_CONFIG**: Carpeta donde se guardará configuración de pihole
- **VOL_MEDIA**: Carpeta de media
