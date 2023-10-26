# Elementos multimedia
***
## Índice
- [Audio](#audio)
- [Viedeo](#video)
***
## Audio
Para agregar un audio utilizamos la etiqueta `audio` esta etiqueta es una etiqueta de línea. 
```html
<audio src="medio/archivo_audio.mp3" controls></audio>
```
Los formatos más comunes para esta etiqueta son el mp3 y mp4

Algunos atributos útiles al usar esta etiqueta
- `autoplay` --> este atributo permite iniciar el audio una vez que se cargue el navegador
- `loop` --> este permite repetir el audio una vez que haya terminado
- `muted` --> este atributo permite iniciar el audio muteado.
- `preload` --> permite precargar el audio una vez que se cargue el sitio, esto ayuda a no esperar a que se vaya cargando el audio.
## Video
Para agregar un video utilizamos la etiqueta `video` esta etiqueta es una etiqueta de línea

```html
<video src="media/archivo_video.mp4"></video>
```

Al igual que en un audio los archivos más comunes son el mp3 y mp4

Los atributos de esta etiqueta son los mismos que en la etiqueta audio

- `poster` --> permite cargar una imágen como miniatura del video.