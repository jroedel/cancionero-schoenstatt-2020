# Cancionero Schoenstatt 2020

**Objetivo**: Convertir el archivo del P. Tute a format Chordpro en archivos
individuales para ser importado a https://schoenstatt.link/music

**Método**:

1. Traducir el archivo de DOCX a markdown:
`pandoc --to=markdown -o Cancionero.markdown Cancionero2020.docx`
2. Crear la lista de canciones en CSV para ir agregando metadatos en Google
Sheets
3. Separar las canciones en archivos distintos según el encabezamiento 3.
python regex
4. Compilar una lista de acordes para que los músicos digan a que traducen en
acordes A-G
5. Aplicar regex para:
  * Dejar el título en formato Chordpro
  * Eliminar espacios extra entre líneas
  * Identificar el estribillo por el uso de \*
  * Traducir acordes del francés al estandar y ponerlos en formato Chordpro
6. El resto será manual
