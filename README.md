# CODE QUEST V3 · Ingeniería en Sistemas PUCE

Aplicación educativa para la casa abierta. Versión 3.0.1, publicada como proyecto independiente de la V2.

- [Abrir e instalar la aplicación](https://thesteppenwolf.github.io/code-quest-puce-v3/)
- [Ver la presentación para celular](https://thesteppenwolf.github.io/code-quest-puce-v3/ver-celular.html)

Incluye retos de programación, mapas aleatorios, Diseña y entrena, Tú vs la IA, música instrumental opcional y controles con mayor separación. El editor conserva su posición al añadir acciones.

## Instalación para visitantes

Escanear el QR y abrir en Chrome para Android. Elegir Instalar aplicación o Agregar a la pantalla principal en el menú del navegador. En iPhone, abrir en Safari y usar Compartir → Agregar a Inicio. La aplicación conserva sus recursos para los siguientes usos sin conexión.

## Código fuente y publicación

El archivo `CODE_QUEST_Android_v3.zip.b64` contiene el paquete completo de código fuente, pruebas y recursos, codificado como texto para conservarlo en GitHub. GitHub Actions lo reconstruye, verifica su SHA-256, ejecuta las comprobaciones y publica su carpeta `dist` en Pages. El flujo tiene acceso de lectura al contenido del repositorio.

Para recuperar el ZIP con Python 3:

```sh
python -c "import base64,pathlib; pathlib.Path('CODE_QUEST_Android_v3.zip').write_bytes(base64.b64decode(pathlib.Path('CODE_QUEST_Android_v3.zip.b64').read_bytes()))"
```

SHA-256 del ZIP: `5e987e5369d6eb916a1a528d3b36a6117e7be58983a715e0f25ce3f03b6d5e00`.

Descomprimir el ZIP, entrar en `CODE_QUEST_Android_v3` y ejecutar con Node.js 22:

```sh
npm run check
npm test
```

Para servirlo localmente, publicar la carpeta `dist` con un servidor estático. La instalación y el service worker requieren HTTPS o localhost.

La captura de la pantalla publicada se conserva en `docs/CODE_QUEST_v3_celular.jpg.b64` con la misma codificación Base64.

El sitio permanecerá disponible mientras este repositorio y GitHub Pages sigan activos.
