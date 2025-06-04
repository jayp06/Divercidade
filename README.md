# 🎲 Divercidade

**Divercidade** é um jogo de tabuleiro eletrônico baseado no clássico estilo de "jogos de propriedades", onde até 4 jogadores competem para acumular riquezas, comprar propriedades e sobreviver aos desafios do tabuleiro!

---

## ✅ Resumo do Jogo

### 🎯 Objetivo
- Acumular **R$3000** em saldo ou ser o **último jogador ativo** (não falido).

---

## 👥 Jogadores
- De **1 a 4 jogadores**.
- Número de participantes selecionado e **confirmado com botões físicos** no início da partida.

---

## 📋 Estrutura do Tabuleiro
- **24 casas**:
  - **Propriedades** compráveis.
  - Casas de **eventos**: "Sorte ou Revés" e "Feriado".
  - Casa especial: **"Jaula"** (prisão).
  - Casa: **"Vá para Jaula"**.

---

## ⚙️ Mecânicas do Jogo

### 🎲 Movimentação
- Jogadores rolam um **dado virtual** (valor aleatório de 1 a 6).
- Movimentam-se pelo tabuleiro conforme o valor sorteado.

---

### 🏠 Propriedades
- Propriedades podem ser **compradas** se estiverem livres.
- Jogadores pagam **aluguel** ao caírem em propriedades alheias.

---

### 🏗️ Construção
- Proprietários podem construir:
  - Até **3 "casinhas"**.
  - Depois, uma **"mansão"**.
- Construções aumentam o **valor do aluguel**.

---

### 💰 Saldo
- Cada jogador começa com **R$1000**.
- Passar pela casa **"Início"** concede **R$200**.

---

### 🚨 Jaula
- Jogadores podem ser enviados à **"Jaula"**:
  - Perdem **1 turno**.

---

### 🎭 Sorte ou Revés
- Casas que geram **eventos aleatórios**:
  - Ganho ou perda financeira.
  - Movimento extra.
  - Ir para a Jaula.

---

### 🎉 Feriado
- Casa especial que concede um **bônus em dinheiro**.

---

### 💥 Falência
- Jogadores com saldo **negativo** são **eliminados**.
- Suas **propriedades são liberadas**.

---

## 🔧 Interação com o Jogador

### 📺 Display
- Utiliza um **LCD I2C 20x4** para exibir:
  - Informações do jogo.
  - Status dos jogadores.
  - Mensagens de eventos e opções.

---

### 🕹️ Botões

| Função                                           | Pino |
|--------------------------------------------------|------|
| Avançar, não comprar/construir                   | 7    |
| "Sim" (comprar/construir)                        | 9    |
| Seleção do número de jogadores                   | 12   |
| Confirmação da quantidade de jogadores           | 8    |

---

### 💡 Fita de LED (NeoPixel)
- Conectada ao **Pino 3**.
- Composta por **80 LEDs**:
  - **3 LEDs por casa** do tabuleiro → totalizando 72.
  - **8 LEDs extras** para efeitos especiais.

#### ✨ Funções:
- Indicação visual da **posição dos jogadores** por cor.
- Efeitos visuais para:
  - **Vitória**.
  - **Sorte ou Revés**.
  - **Compra ou construção**.
- Ao alcançar a **última casa**, acendem-se os **3 LEDs da casa** e os **8 LEDs extras**.

---

## 📚 Bibliotecas Utilizadas

### 1️⃣ `Wire.h`
- Comunicação via **I2C** com o **LCD**.

### 2️⃣ `LiquidCrystal_I2C.h`
- Controle simplificado do **display LCD** I2C.

### 3️⃣ `Adafruit_NeoPixel.h`
- Controle da **fita de LED RGB endereçável** para efeitos visuais dinâmicos.

---

## 🛠️ Componentes Eletrônicos

- **Arduino UNO** ou compatível.
- **Display LCD 20x4 com módulo I2C**.
- **Fita de LED NeoPixel** (80 LEDs).
- **Botões táteis** (4 unidades).
- **Resistores** para os botões.
- **Fonte de alimentação** adequada para LEDs.
- **Jumpers** e **protoboard** ou PCB.

---

## 🚀 Como Usar

1. **Monte o circuito** conforme o esquema proposto.
2. **Carregue o código** no Arduino via IDE.
3. Selecione o número de jogadores usando os botões.
4. Confirme a quantidade com o botão no **pino 8**.
5. Divirta-se acumulando riquezas e superando os desafios!

---

## 🏆 Créditos
Desenvolvido como um projeto de integração de:
- Programação em **Arduino**.
- **Eletrônica** digital.
- **Design de jogos** interativos.

---

## 📜 Licença
Este projeto está licenciado sob a **MIT License**.

---

## 📸 Imagens e Vídeos
> _()_

---


