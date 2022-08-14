# canvas
canvas é como uma tela em branco, que com o JS consigo pintar, a tela.
tenho criar uma var tela = no mundo HTML é chamala no JS com o querySelector(canvas);
Faço o uso da var pincel = tela.getContext("") entre os parêntese coloco as opções que são (2d,3d) e por ai vai.

fillStyle = recebe uma cor válida.
fillReact = onde desejo começar a pinta, e o tamanho da tela (X0, Y0, 200 ,240) sempre lembrando que a  fillStyle, semore vem primeiro por ser a cor.


# CANVAS
pincel.beginPath(); - Criar o caminho ao qual, vai ser desenhado o caminho,
pincel.arc(x, y, 10, 0, 2 * 3.14); - Aqui passo as coordenadas do desenho. com parte final em redianos 3.14 famoso (Pi);

Função responsavel ao clique do botão direito do mouse. É o (.oncontextmenu = mudaCor;)