🎲 Divercidade: Sobre o Jogo e Bibliotecas
✅ Resumo do Jogo
🎯 Objetivo
Acumular uma riqueza de R$3000
ou

Ser o último jogador ativo (não falido) no tabuleiro.

👥 Jogadores
De 1 a 4 jogadores.

Selecionáveis no início da partida por meio de botões.

📋 Tabuleiro
Composto por 24 casas:

Propriedades compráveis.

Casas de eventos: "Sorte ou Revés" e "Feriado".

"Jaula" (prisão).

Casa "Vá para Jaula".

⚙️ Mecânicas Principais
🎲 Movimentação
Jogadores rolam um dado virtual (valor aleatório de 1 a 6).

Movem-se pelo tabuleiro conforme o valor sorteado.

🏠 Propriedades
Jogadores podem comprar propriedades livres.

Se caírem em propriedade de outro jogador, devem pagar aluguel.

🏗️ Construção
Donos podem construir:

Até 3 "casinhas".

Depois, uma "mansão".

Construções aumentam o valor do aluguel.

💰 Saldo
Cada jogador começa com R$1000.

Ao passar pelo "Início", recebe um bônus de R$200.

🚨 Jaula
Jogadores podem ser enviados para a "Jaula":

Ficam presos.

Perdem 1 turno.

🎭 Sorte ou Revés
Casas especiais que acionam eventos aleatórios:

Ganhos ou perdas financeiras.

Movimentação extra.

Ir para a Jaula.

🎉 Feriado
Casa especial que concede um bônus em dinheiro.

💥 Falência
Se o saldo ficar negativo:

O jogador é eliminado.

Suas propriedades são liberadas.

🔧 Interação
📺 Display
Um LCD I2C 20x4 exibe:

Informações do jogo.

Status dos jogadores.

Eventos e opções.

🕹️ Botões
Função	Pino
Avançar jogo / Não comprar ou construir	7
Sim (comprar/construir) / Confirmar seleção	9
Seleção do número de jogadores	12

💡 Fita de LED (NeoPixel)
Conectada ao Pino 3.

80 LEDs no total:

3 LEDs por casa do tabuleiro → 72 LEDs.

8 LEDs extras para efeitos especiais.

✨ Funções da fita:
Indicar a posição de cada jogador com sua cor.

Quando um jogador atinge a última casa:

Acendem os 3 LEDs da casa e os 8 LEDs extras.

Efeitos visuais para:

Vitória.

Sorte ou Revés.

Compra.

Construção.

📚 Bibliotecas Utilizadas
1️⃣ Wire.h
Comunicação via protocolo I2C.

Usada para interagir com o display LCD.

2️⃣ LiquidCrystal_I2C.h
Controle de displays LCD com módulo conversor I2C.

Simplifica a conexão e o controle do display.

3️⃣ Adafruit_NeoPixel.h
Controle de fitas de LED RGB endereçáveis (ex.: WS2812B, SK6812).

Permite criar efeitos de iluminação dinâmicos.

