# Prueba de Script con Bootstrap

Este es un ejemplo simple de un documento HTML que utiliza Bootstrap y JavaScript para generar botones y realizar un seguimiento de los clics.

## Contenido del Documento

1. **Inclusión de Bootstrap CSS:** Se incluye el archivo CSS de Bootstrap para estilos predefinidos.
2. **Estilos Personalizados:** Se define un estilo personalizado para cambiar el color de fondo de los botones al hacer clic.
3. **Script de Simulación de Clics:** Se agrega un script que obtiene una lista de botones y simula un clic en cada uno de ellos.
4. **Generación de Botones:** Se genera un bloque de 100 botones organizados en un grid de 10 columnas utilizando Bootstrap.
5. **Manejo de Clics y Seguimiento:** Se utiliza JavaScript para manejar los clics en los botones y realizar un seguimiento de los botones clicados.
6. **Inclusión de Bootstrap JS y Popper.js:** Se incluyen los archivos JavaScript necesarios para el funcionamiento de algunos componentes de Bootstrap.

## Cómo Probar

1. Descarga este archivo HTML.
2. Abre el archivo en un navegador web.
3. Observa cómo se generan y manipulan los botones.

## Notas Adicionales

- Se utiliza la clase `btn-clicked` para cambiar el color de fondo de un botón después de hacer clic.
- Los botones clicados se registran en la consola del navegador.

## Requisitos

- Conexión a Internet (para cargar Bootstrap CSS y JS desde CDN).
- Navegador web compatible con Bootstrap y JavaScript.


Ispirated and thanks to [BryanHaley](https://gist.github.com/BryanHaley) for this.
```javascript
setInterval(function () {
    video = document.getElementsByTagName('ytd-playlist-video-renderer')[0];

    video.querySelector('#primary button[aria-label="Action menu"]').click();

    var things = document.evaluate(
        '//span[contains(text(),"Remove from")]',
        document,
        null,
        XPathResult.ORDERED_NODE_SNAPSHOT_TYPE,
        null
    );

    for (var i = 0; i < things.snapshotLength; i++) 
    {
        things.snapshotItem(i).click();
    }
}, 500);
```

Non-english users will need to change "Action menu" and "Remove from" to what YouTube uses for their localization.
