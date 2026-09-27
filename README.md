⚔️ RPG — Dragon Repeller

Um jogo de RPG em texto, jogado direto no navegador, feito com HTML, CSS e JavaScript puro. O projeto foi desenvolvido a partir do desafio "Learn Basic JavaScript by Building a Role Playing Game" do freeCodeCamp.

Mostrar Imagem Mostrar Imagem Mostrar Imagem

📖 Sobre o jogo

Um dragão impede que as pessoas saiam da cidade, e cabe a você derrotá-lo. Partindo da praça central, você pode visitar a loja para comprar vida e armas, enfrentar monstros na caverna para ganhar ouro e experiência e, quando estiver pronto, desafiar o dragão.

Toda a interface é controlada por três botões, cujos textos e ações mudam conforme o local em que o jogador está.

🎮 Como jogar

O jogador começa com:

XP	Vida	Ouro	Arma
0	100	50	Graveto (stick)
🏘️ Locais
Praça da cidade: ponto de partida. Dá acesso à loja, à caverna e à luta contra o dragão.
Loja: compra de vida e de armas.
Caverna: luta contra monstros mais fracos para ganhar ouro e XP.
🛒 Loja
Ação	Custo	Efeito
Comprar vida	10 de ouro	+10 de vida
Comprar arma	30 de ouro	Recebe a próxima arma da lista
Vender arma	—	+15 de ouro (disponível ao ter a arma mais forte)
🗡️ Armas
Arma	Poder
Stick (graveto)	5
Dagger (adaga)	30
Claw hammer (martelo)	50
Sword (espada)	100
👹 Monstros
Monstro	Nível	Vida
Slime	2	15
Fanged beast	8	60
Dragon (chefe final)	20	300
⚔️ Combate

Durante uma luta, o jogador pode atacar, esquivar ou fugir de volta para a cidade.

Dano do jogador: poder da arma + um bônus aleatório baseado no XP.
Dano do monstro: nível × 5, reduzido por um valor aleatório baseado no XP do jogador.
Chance de acerto: 80%. Com menos de 20 de vida, o jogador sempre acerta.
Quebra de arma: a cada ataque, há 10% de chance de a arma atual quebrar (exceto quando ela é a única do inventário).
Recompensa: ao derrotar um monstro, o jogador ganha XP igual ao nível dele e ouro proporcional a esse nível.

Se a vida chegar a zero, o jogo acaba. Derrotar o dragão vence o jogo. Nos dois casos, é possível recomeçar do zero.

🥚 Easter egg

Depois de derrotar um monstro, há um minijogo secreto: escolha o número 2 ou 8. Dez números aleatórios de 0 a 10 são sorteados. Se o seu número aparecer, você ganha 20 de ouro. Se não aparecer, perde 10 de vida.

🧠 Conceitos praticados
Manipulação do DOM (querySelector, innerText, innerHTML, style)
Eventos com onclick, trocados dinamicamente a cada local
Arrays de objetos para representar armas, monstros e locais
Uma função genérica update() que redesenha a interface a partir dos dados do local
Condicionais, laços (while, for) e operador ternário
Números aleatórios com Math.random() e Math.floor()
Controle do estado do jogo (vida, ouro, XP, inventário)
📁 Estrutura
RPG/
├── index.html   # Estrutura da interface (status, botões e texto)
├── estilo.css   # Estilização do jogo
├── script.js    # Toda a lógica do jogo
└── README.md
🚀 Como executar
Clone o repositório:
bash
   git clone https://github.com/GustavoM-Dev/RPG.git
Entre na pasta do projeto:
bash
   cd RPG
Abra o arquivo index.html no navegador.

Não é preciso instalar nada.

🌐 Jogar online

Com o GitHub Pages ativado, o jogo fica disponível em:

https://gustavom-dev.github.io/RPG/

🔮 Melhorias futuras
Traduzir os textos do jogo para português
Deixar o layout responsivo para celulares
Salvar o progresso com localStorage
Adicionar novos monstros, armas e locais
🙌 Créditos

Projeto baseado no currículo de JavaScript do freeCodeCamp.

👤 Autor

Gustavo — @GustavoM-Dev
