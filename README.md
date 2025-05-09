# 🍄 Mushroom's Land

🎮 **Mushroom's Land** é um jogo de plataforma 2D feito em **JavaScript puro**, utilizando apenas **HTML5 Canvas** e sem bibliotecas de jogos externas.

Seu objetivo é simples: **coletar todas as moedas e se manter vivo!**

---

## 🚀 Como Jogar

- Explore o mapa
- Colete todas as moedas
- Evite cair na água
- Fuja (ou derrote!) as temidas **bolhas de gosma azul**
- Pule sobre os inimigos para derrotá-los
- Ao coletar todas as moedas, você avança para o próximo nível  
> ⚠️ Atualmente, o jogo possui **2 fases** disponíveis.

---

## ⚙️ Controles

| Tecla       | Ação                   |
|-------------|------------------------|
| `W` ou `↑`  | Pular                  |
| `A` ou `←`  | Mover para a esquerda  |
| `D` ou `→`  | Mover para a direita   |

---

## 🛠️ Tecnologias Utilizadas

- **HTML5**: Estrutura da página
- **CSS3**: Estilização básica da interface
- **JavaScript (puro)**: Toda a lógica do jogo
- **Canvas API**: Renderização gráfica
- **GSAP (GreenSock)**: Animações suaves (usado no HUD e efeitos)

---

## 🧱 Estrutura do Projeto

mushrooms_land/
├── audio/ # Trilha sonora e efeitos
├── img/ # Sprites, tilesets, objetos
├── index.html # HTML principal
├── style.css # Estilo básico do jogo
├── script.js # Lógica principal do jogo
├── js/
│ ├── Player.js
│ ├── Enemy.js
│ ├── Level.js
│ ├── Sprite.js
│ └── ...
└── maps/ # Dados dos mapas (fase 1 e 2)


---

## 🧩 Componentes Principais

### 👤 Jogador
- Movimentação com teclado
- Sprites para correr, pular, se machucar e morrer
- Interação com inimigos e moedas

### 👾 Inimigos (Ex: bolhas de gosma)
- Comportamento de patrulha
- Mudam de comportamento ao detectar o jogador
- Podem ser derrotados pulando sobre eles

### 💰 Moedas
- Espalhadas pelo mapa
- Coletáveis para avançar ao próximo nível

### 🗺️ Níveis
- Baseados em mapas com tiles de 16x16 pixels
- Contêm plataformas, moedas e inimigos
- Progresso ao completar os objetivos

### 🧠 HUD (Painel de Informações)
- Corações (vidas)
- Barra de progresso das moedas coletadas
- Botões de pausa e reinício

---

## ⚙️ Mecânicas

- **Gravidade** aplicada ao jogador e inimigos
- **Colisão manual** com plataformas e objetos
- **Animações por frames**, baseadas em contadores
- **Sistema de vida e morte** com reinício automático
- **Transição entre níveis** ao completar objetivos

---

## 🔊 Áudio

Inclui efeitos e música de fundo:

🎵 Trilha sonora ambiente

💥 Efeitos de morte e vitória

🧪 Observações para Desenvolvedores
Muitos parâmetros do jogo, como:

Gravidade

Velocidade do personagem

Vida máxima

Poder de ataque

Podem ser facilmente ajustados nas constantes do arquivo script.js, facilitando personalizações ou melhorias.
