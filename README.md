# EXAMEN P.C
## Artical Pong
### JAVIERA BRAVO
Para la realizacion de este examen quise implementar una estetica de juegos convencionales antiguos que jugaban con efectos visuales simples, pero que definieron la estetica retro, relacionandolo igualmente con mi solemne la cual fue ins´pirada en el optical ART, en este caso con la modalidad de juego el cual tiene la dificultad de un fondo distrayente de ilusion optica.
---------------------------------------------------------------------------------------------------------------------------------------------------------------
¿EN QUE CONSISTE MI PROYECTO?
Mi proyecto consiste en un juego virtual popularmente conocido como PONG, en referencia al ping pong, lo que aprecian en pantalla es una ellipse que representa la pelota y una barra lateral recta que seria la raqueta, de fondo la ya mencionada imagen optica y tambien un marcador de puntaje por cada interaccion entre la pelota y la raqueta.
-------------------------------------------------------------------------------------------------------------------------------------------------------------
INPUTS
Este trabajo cuenta con dos tipos de inputs

1= la input de click en el mouse para comenzar 
// click
function mousePressed() {
  if (estado == 0 || estado == 2) {
    estado = 1;
    marcador = 0;
    posX = random(50, width / 2);
    posY = random(50, height - 50);
    velX = 5;
    velY = 5;
  }
--------------------------------------------------------------------------------------------------
1.2= como segundo input esta el INPUT CONTINUO DEL MOUSE (POSICION)
rect(width - 70, mouseY - 40, 40, 80);

OUTPUTS
#  Outputs del tranajo(salidas)
En este proyecto, los outputs son todos los elementos que el juego **renderiza en pantalla** o **produce como resultado visual**.


###PELOTA
1-javascript
ellipse(posX, posY, 24);
---

##  Elementos visuales
-  Pelota que se mueve por la pantalla
-  Raqueta
-  Imagen de fondo (op art)
-  Estrellas
-  Grilla 

---

## Texto en pantalla
- Menú inicial: "JUEGO" y "Haz clic para comenzar"
- Puntaje: "Puntos: X"
- Pantalla de derrota: "PERDISTE" y "Haz clic para reiniciar"

---

## Estados del juego
- Menú (estado 0)
- Juego activo (estado 1)
- Derrota (estado 2)

---

CONCEPTO
Mi concepto principal fue el arte optico y los juegos vintage, tambien me inpire en Allan Alcor quien creo que el juego original de Pong en 1972 como un simple proyecto de prueba sin imaginarse que se convertiria en un juego iconico de la epoca.

INTERACCIONES
El juego se centra en dos interacciones clave: el movimiento de la raqueta utilizando el mouse y un clic para iniciar o reiniciar el juego. El objetivo principal es mantener la pelota en juego durante el mayor tiempo posible.

###  Datos del mouse
- `mouseY` posición vertical del mouse
- clic del mouse `mousePressed

### Datos generados por el sistema

- posiciones aleatorias de la pelota:
- `posX = random`
- `posY = random`

### Datos internos del juego

- `estado`
- `marcador`

- velocidad de la pelota:
- `velX`
- `velY`

## Procesamiento de datos

El juego procesa los datos dentro de `draw` en cada frame:

###  Movimiento de la pelota
- La posición cambia constantemente:
```javascript posX += velX;
posY += velY;
------------------------------------------------------------------------------------------------------------------------

##RECURSOS
Se uso el recurso de imagen para el fondo en formato jpg que añade la funcion de dificultad en el juego, ya que distrae y camufla la raqueta y pelota.

##REFLEXION
Este proyecto permitió comprender cómo un videojuego no es solo un conjunto de imágenes en movimiento, sino un sistema donde los datos entran, se procesan y generan resultados en tiempo real.
A través del desarrollo del juego tipo Pong en p5.js, se pudo observar cómo el movimiento del mouse, los clics y las variables internas como la posición, velocidad y puntaje trabajan en conjunto para crear una experiencia interactiva.
También fue importante entender el uso de los estados del juego , ya que permiten organizar la lógica y dar estructura a la interacción del usuario.
En conclusión, este proyecto ayudó a comprender de manera práctica conceptos básicos de programación como variables, condicionales, bucles y eventos, además de mostrar cómo estos elementos pueden utilizarse para crear una experiencia jugable completa e interactiva.
