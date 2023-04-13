# speech_recognition
transcripcion automatica


Este código en Python utiliza las bibliotecas speech_recognition, pydub y concurrent.futures para transcribir un archivo de audio en formato m4a a texto. Primero, el archivo de audio se carga y se convierte en formato WAV para facilitar la manipulación. Luego, el audio se divide en trozos de 10 segundos para procesarlos en paralelo y mejorar la eficiencia.

La función "transcribir" se define para transcribir cada trozo de audio a texto utilizando la API de reconocimiento de voz de Google. Si la transcripción no es posible para un trozo de audio, se pasa al siguiente.

Después, se crea un conjunto de trabajadores para procesar los trozos de audio en paralelo y se ejecuta la función "transcribir" para cada trozo de audio. El texto generado por cada trabajador se agrega a una cadena de texto.

Finalmente, se escribe la transcripción completa en un archivo de texto y se guarda en el sistema de archivos.


El principal uso que le daré es para transcribir las clases que tomo en la escuela.
