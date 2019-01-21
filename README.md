En el ejercicio XSS STORED de DVWA, podemos alterar el código fuente o insertar script:

Dónde el código es: XSS-STORE-INICIAL.txt
Sanitizamos los mensajes y nombres de entrada con lo siguiente:

![image](https://user-images.githubusercontent.com/46895869/51488793-836ecf80-1d74-11e9-9ba3-0c15ca4a21bf.png)

Usamos strip_tags para eliminar las etiquetas HTML de las cadenas que se envían a PHP desde el navegador. Mejor aún, también puede almacenar de forma segura los mismos datos sin pasarlos por strip_tags si usa htmlspecialchars para escapar de cualquier carácter que pueda delimitar las etiquetas cuando envíe los datos de vuelta al navegador.
Dónde el código es: XSS-STORE-FINAL.txt
