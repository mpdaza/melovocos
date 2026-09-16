# MeloVOCOS · Iberspeech 2026

Página estática en inglés, sin compilación ni dependencias externas, preparada para GitHub Pages.

## Estructura
- index.html: contenido y JavaScript mínimo para copiar la cita.
- assets/style.css: diseño adaptable a escritorio y móvil.
- assets/paper-figure-1.png: Figura 1 original extraída del PDF en alta resolución.
- assets/audio/: carpeta para las muestras de voz.
- paper.pdf: copia del manuscrito proporcionado.

Se conserva la organización de paper22: presentación, introducción técnica, resultados, comparación, audios, método y cita. El diseño es independiente.

## Ver localmente
Abrir index.html en el navegador. El contenido funciona sin servidor y sin conexión. El botón de cita selecciona el texto si el navegador no permite acceder al portapapeles desde un archivo local.

## Publicar en GitHub Pages
Subir el contenido de esta carpeta a la raíz del repositorio destinado a la página y configurar GitHub Pages para servir esa raíz. También puede alojarse como subcarpeta de un sitio: todos los enlaces son relativos. No hace falta npm, Jekyll ni compilación.

## Incorporar audios
No se han proporcionado audios. La sección muestra su disponibilidad real y no solicita archivos inexistentes.
1. Copiar los WAV o MP3 a assets/audio/.
2. En cada tarjeta, reemplazar las filas pendientes por elementos con etiqueta y reproductor. Comparar la misma frase entre referencia, MeloTTS y MeloVOCOS.
3. Ejemplo, solo después de añadir el archivo correspondiente:

<article>
  <h4>Reference · Male speaker</h4>
  <audio controls preload="none" aria-label="Reference speech, male speaker">
    <source src="assets/audio/male-reference.wav" type="audio/wav">
    Your browser does not support audio playback.
  </audio>
</article>

4. Actualizar «Pending audio» y «Audio samples are not yet available». Añadir la transcripción de cada frase cuando esté disponible.
El JavaScript incluido pausa los otros reproductores al iniciar uno.

## Metadatos y fidelidad al artículo
Autores confirmados por la usuaria: María Pilar Daza LLin, Jose Luis Blanco y Luis Hernandez Gomez. Figuran en la cabecera, los metadatos y la cita. El PDF conserva la versión original proporcionada. La cita es provisional hasta disponer de los datos de publicación.

Los datos de eficiencia reproducen la Tabla 5: 27.45 h / 1260 épocas / 78.4 s por época y 6.63 h / 300 épocas / 79.6 s por época. La reducción se describe como aproximadamente 4.2× siguiendo el artículo, con el cociente de tiempo 4.14× aclarado. El encabezado muestra una adaptación visual de la Figura 1; la extracción original sigue disponible mediante enlace.

No se ha publicado ni vinculado esta carpeta a ningún repositorio remoto.


## Congreso e identidad visual
- IberSPEECH 2026: 18–20 de noviembre de 2026, Madrid.
- Sede: ETSIT-UPM, Avenida Complutense 30, 28040 Madrid.
- Fuentes: https://iberspeech.tech/2026/ y https://iberspeech.tech/2026/venue/
- Logo oficial GAPS: https://www.gaps.ssr.upm.es/images/04_logotipo_GAPS.png (copia local sin recolorear).
- assets/paper-figure-1-styled.png: adaptación visual de la Figura 1 a la paleta de la web. El enlace «Original figure» conserva acceso a la extracción original.
