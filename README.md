

# Divercidade: sobre o jogo e biblioteca 🎲


Resumo do Jogo
Objetivo: Acumular uma riqueza de R$3000 ou ser o último jogador ativo (não falido) no tabuleiro.
Jogadores: Permite de 1 a 4 jogadores, selecionáveis no início da partida através de botões.
Tabuleiro: Consiste em 24 casas, cada uma com diferentes propriedades compráveis, casas de eventos ("Sorte ou Revés", "Feriado"), a "Jaula" (prisão), e a casa "Vá para Jaula".
Mecânicas Principais:
Movimentação: Jogadores rolam um dado virtual (número aleatório de 1 a 6) para se moverem pelo tabuleiro.
Propriedades: Podem comprar propriedades não possuídas. Se caírem em uma propriedade de outro jogador, pagam aluguel.
Construção: Donos de propriedades podem construir "casinhas" (até 3) e depois uma "mansão" em suas propriedades, aumentando o valor do aluguel.
Saldo: Cada jogador começa com R$1000. Passar pelo "Início" concede R$200.
Jaula: Jogadores podem ser enviados para a "Jaula" e perdem 1 turno.
Sorte ou Revés: Casas especiais que acionam eventos aleatórios que podem resultar em ganhos/perdas financeiras, movimentação extra ou ida para a Jaula.
Feriado: Uma casa especial que concede um bônus em dinheiro.
Falência: Se o saldo de um jogador se tornar negativo, ele é eliminado do jogo e suas propriedades são liberadas.
Interação:
Display: Um LCD I2C 20x4 exibe informações do jogo, status dos jogadores, eventos e opções.
Botões:
Pino 7: Usado para avançar o jogo, não comprar/construir, e confirmar mensagens.
Pino 9: Usado para "Sim" (comprar/construir) e para confirmar a seleção do número de jogadores.
Pino 12: Usado para selecionar o número de jogadores no início da partida.
Fita de LED (NeoPixel): Conectada ao Pino 3, com 80 LEDs (3 LEDs por casa do tabuleiro + 8 LEDs extras). Indica a posição de cada jogador ativo no tabuleiro com sua cor respectiva. Quando um jogador atinge a última casa, os 3 LEDs da casa e os 8 LEDs extras acendem. Efeitos visuais também ocorrem para eventos como vitória, Sorte/Revés, compra, construção, etc.
Bibliotecas Utilizadas 📚
O código utiliza as seguintes bibliotecas Arduino:

Wire.h: Essencial para a comunicação via protocolo I2C, usada para interagir com o display LCD.
LiquidCrystal_I2C.h: Biblioteca específica para controlar displays LCD que utilizam um módulo conversor I2C, simplificando a conexão e o controle do display.
Adafruit_NeoPixel.h: Biblioteca da Adafruit para controlar fitas de LED RGB endereçáveis individualmente (como WS2812B, SK6812, etc.), permitindo efeitos de iluminação dinâmicos.
