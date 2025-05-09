# Sobre o Jogo
Este é um jogo de plataforma simples em JavaScript puro, sem usar bibliotecas, apenas HTML Canvas. <br>
Seu objetivo é se mover pelo mapa e coletar todas as moedas para avançar para a próxima fase. <br>
Mantenha-se vivo, não caia na água e não seja atacado pelas terríveis bolhas de gosma azul! <br>
As bolhas de gosma parecerão dormentes, mas começarão a se mover em sua direção se você entrar em seu campo de visão. <br>
Você pode se livrar delas pulando sobre elas. <br>
(Até o momento, existem duas fases.) <br>
 

__Observação__:
Muitos controles importantes, como gravidade, velocidade, vida máxima, poder de ataque, etc., podem ser controlados usando as constantes
que são definidas no início de script.js.

__Guia de Desenvolvimento do Jogo Mushroom's Land__:

Visão Geral

Mushroom's Land é um jogo de plataforma 2D desenvolvido utilizando HTML5, JavaScript puro e a tag <canvas> do HTML para renderização dos gráficos. O jogo foi concebido para simular um ambiente clássico de aventura, com um personagem principal que coleta moedas, derrota inimigos e avança por diferentes níveis.

Tecnologias Utilizadas

HTML5: Estrutura do documento.

CSS3: Estilização básica (pouco utilizado).

JavaScript: Toda a lógica do jogo é escrita em JS puro.

Canvas API: Para renderização de sprites, cenários e animações.

GSAP (GreenSock Animation Platform): Biblioteca para animações suaves (usada no HUD e efeitos).

Estrutura do Projeto

mushrooms_land/
|-- audio/                      # Arquivos de som (trilha, efeitos)
|-- img/                        # Sprites e folhas de sprites (tilesets, inimigos, etc)
|-- index.html                  # HTML principal
|-- style.css                   # CSS básico
|-- main.js                     # Arquivo principal com a lógica do jogo
|-- classes/                    # Classes JavaScript (Player, Level, Enemy, Sprite, etc)
|-- maps/                       # Dados dos mapas e posicionamento

Componentes Principais

1. Player (Jogador)

Controlado por teclado (WASD ou setas).

Possui sprites para diferentes estados: parado, correndo, machucado e morto.

Pode pular, se mover e interagir com inimigos e moedas.

2. Inimigos

Exemplo: "Skelly" (Esqueleto).

Possuem comportamentos simples de patrulhamento.

Têm sprites para andar, atacar e morrer.

3. Moedas

Dispostas no cenário.

Ao serem coletadas, aumentam a barra de progresso do nível.

4. Níveis

Representados por mapas com tiles (16x16 px).

Cada nível possui um background, plataformas, moedas e inimigos.

Avanço automático ao coletar todas as moedas.

5. HUD (Heads-Up Display)

Exibe corações (vidas), barra de progresso de moedas e informações de jogo.

Mecânicas do Jogo

Gravidade: Aplicada ao jogador e inimigos para simular queda.

Colisão com plataformas: Verificações manuais para detectar se o jogador está pisando ou batendo em blocos.

Animações: Alternação de frames com base em um contador (animationSpeed).

Morte e Ressurreição: O jogador pode morrer ao ser atingido, e é reiniciado com vidas.

Sistema de Som

Inclui efeitos de morte, vitória e uma trilha sonora de fundo:

const backgroundMusic = new Audio('./audio/mystic_journey.mp3');
backgroundMusic.loop = true;
backgroundMusic.volume = 1.0; // Volume ajustado

Controles

W / ArrowUp: Pular

A / ArrowLeft: Mover para a esquerda

D / ArrowRight: Mover para a direita

Espaço: (Reserva para ataque no futuro)



Boa sorte :)
