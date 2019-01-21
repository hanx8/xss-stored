En el ejercicio XSS STORED de DVWA, podemos alterar el código fuente o insertar script:

![image](https://user-images.githubusercontent.com/46895869/51488994-03953500-1d75-11e9-9770-fc9149cb2519.png)


![image](https://user-images.githubusercontent.com/46895869/51489062-34756a00-1d75-11e9-9757-56dbf7174223.png)

Dónde el código es: XSS-STORE-INICIAL.txt

Sanitizamos los mensajes y nombres de entrada con lo siguiente:

![image](https://user-images.githubusercontent.com/46895869/51488793-836ecf80-1d74-11e9-9ba3-0c15ca4a21bf.png)

Usamos strip_tags para eliminar las etiquetas HTML de las cadenas que se envían a PHP desde el navegador. Mejor aún, también puede almacenar de forma segura los mismos datos sin pasarlos por strip_tags si usa htmlspecialchars para escapar de cualquier carácter que pueda delimitar las etiquetas cuando envíe los datos de vuelta al navegador.

 
Dónde el código es: XSS-STORE-FINAL.txt
Luego de la corrección, ya no se modifica el texto insertado ni se inserta el script:

