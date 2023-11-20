# EXAMEN PRIMERA EVALUACION

## Introduccion

Este documento es una pequeña memoria realizada para el examen de la primera evaluacion de DAW, este examen consta de 4 ejercicios.
1. Test de preguntas teoricas: (3 puntos)
2. SSH + Comand lines (3 puntos)
3. Virtualhost (2 puntos)
4. Documentacion + Github(2 puntos)
   
Mas adelante explicare cada uno de estos 4 puntos por separado.


**Contexto:** Este proyecto se realiza en situación de un **examen** para la asignatura de **DAW** , concretamente de las 15:00 de la terde a las 18:30 con un total de **3 horas y media** para realizar los 4 ejercicios.Utilizaremos las erramientas de ubuntu y su terminal para realizar la mayoria de los ejercicios ademas de guithub.

**Motivacion:** Aprobar esta asignatura ademas de conseguir mas conocimientos sobre **cliente-servidor** y **apache** en general

Ahora si empezemos con la explicacion de los pasos a seguir en cada ejercicio:

## EJERCICIO 1
Simplemente contestar las perguntas que hay en el test teiendo en cueanta que los aciertos suman 0.3 y los fallos restan 0,1.

## EJERCICIO 2
En este ejercicio teniamos que seguir el siguiente enunciado:
>Documenta todos los pasos realizados en un archivo MarkDown. Accede a esta máquina remota mediante ssh:
Deberás ir al escritorio y crear un archivo de texto que contenga como nombre de archivo, tu nombre propio y apellido sin espacios y con extensión txt (por ejemplo ArnoldSchwarzenegger.txt) escribe en su interior el resultado de whoami.
Después, mediante otro comando, concatena al final del archivo el resultado del comando necesario para saber quién >está conectado a la máquina mediante ssh.

Para realizarlo he seguido los siguientes pasos:

1. Contectarme al servidor mediante ssh:![conectarme al servidor](https://github.com/IvanYeste/ExamenDAW/blob/main/ConectarSSH.png)
2. Crear el archivo en el escritorio del servidor: ![crear archivo ](https://github.com/IvanYeste/ExamenDAW/blob/main/EscribirArchivo.png)
3. Escribir contenido en el mediante el editor de texto nano, en este caso havia que escribir el resultado del comando *'whoami'*
4. Concatenar al texto del archivo el resultado del comando *'who'* para saber quein esta conectado ![concatenar](https://github.com/IvanYeste/ExamenDAW/blob/main/Concatenar.png)
5. Desconectarme del servidor y listo.


## EJERCICIO 3
En este ejercicio teniamos que seguir el siguiente enunciado:
>Documenta todos los pasos realizados en un archivo MarkDown. Crea en tu máquina un virtualhost donde escribiendo “daw.ejercicio3.com” nos envíe a una web local que simplemente contenga tu nombre. No cierres la máquina al acabar el >examen para poder comprobar su funcionamiento.

Y para realizarlo he siguido los siguientes pasos
1. Crear una carpeta con el siguiente comando `sudo mkdir /var/www/gci`
2. Crear un archivo html con el editor de textos nano ![modificarhtml](https://github.com/IvanYeste/ExamenDAW/blob/main/modificarhtml.png)
3. Devemos ejecutar estos tres comandos `cd /etc/apache2/sites-available/` `sudo cp 000-default.conf gci.conf` `sudo nano gci.conf` para crear el archivo de configuracion
4. Modificamos el archivo de configuracion de la siguiente manera: ![modificar config](https://github.com/IvanYeste/ExamenDAW/blob/main/modificarconfig.png)
5. Modificar el archivo hostsañadiendo la 3 linea de texto de la imagen: ![modificarhosts](https://github.com/IvanYeste/ExamenDAW/blob/main/modificarelarchivohost.png)
6. Una vez hechos estos pasos se puede acceder a la pagina web creada poninendo el el buscador *daw.ejercicio3.com*


## EJERCICIO 4
En este ejercicio teniamos el siguiente enunciado:
>Recopila todos los ejercicios anteriores en un documento estilo memoria. Además, entrégalo todo subiéndolo a tu >Github personal y haciéndolo público. Envía el link del repositorio en la entrega.

Que basicamente es lo que he hecho en este repositorio asi que no creo que tenga que explicar nada mas.


## Conclusión
Ha sido un examen ligero ya que la **dificultad no era muy elevada** aunque se tiene que tener algo de conocimiento previo sobre el tema y no solo mirar los apuntes ya que sino te puedes atascar en algun paso.



