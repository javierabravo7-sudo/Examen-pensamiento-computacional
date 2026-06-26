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

