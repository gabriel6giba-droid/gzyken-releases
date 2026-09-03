# Descargas de GZyken Launcher

Este repositorio no tiene código. Existe para una sola cosa: **alojar los ejecutables**
de GZyken Launcher como assets de cada Release, con una URL estable y sin límite de
ancho de banda.

👉 **[Ir a la última versión](https://github.com/gabriel6giba-droid/gzyken-releases/releases/latest)**

La página de descargas, con los requisitos y las sumas de verificación, está en el sitio
de GZyken.

## Por qué acá y no en el sitio web

Los instaladores pesan más de 100 MB cada uno. Servirlos desde el hosting del sitio
gastaría la cuota de ancho de banda y obligaría a resubirlos en cada despliegue. Los
assets de una Release viven fuera del historial de git y los sirve el CDN de GitHub.

## Verificar lo que bajaste

Cada Release publica las sumas SHA-256 de sus archivos. En PowerShell:

```powershell
Get-FileHash GZyken-Launcher-0.4.0-portable.exe -Algorithm SHA256
```

El resultado tiene que coincidir con el de las notas de la versión. Si no coincide, no
lo ejecutes.
