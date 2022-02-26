# Docker Pi-hole

<p align="center">
    <a href="https://pi-hole.net/">
        <img src="https://pi-hole.github.io/graphics/Vortex/Vortex_with_Wordmark.svg" width="150" height="260" alt="Pi-hole">
    </a>
    <br>
    <strong>Network-wide ad blocking via your own Linux hardware</strong>
</p>

The Pi-hole® is a DNS sinkhole that protects your devices from unwanted content without installing any client-side software.

## Template

Title: pihole

Description: DNS sinkhole

Icon URL:
https://pi-hole.github.io/graphics/Vortex/Vortex_with_Wordmark.svg
<img src="https://pi-hole.github.io/graphics/Vortex/Vortex_with_Wordmark.svg" width="30" height="30" alt="Pi-hole">

Platform: Linux

Type: Standalone

## Variables de entorno importantes
Al crear el stack

```env
TZ=America/Lima
WEBPASSWORD=
VOL_CONFIG=
```

- **TZ**: Timezone
- **WEBPASSWORD**: Contraseña de la web de pihole
- **VOL_CONFIG**: Carpeta donde se guardará configuración de pihole
