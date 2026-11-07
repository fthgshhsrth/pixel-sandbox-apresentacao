# Pixel Sandbox

RPG de mundo aberto em pixel art, com personagens em 2D dentro de um mundo em 3D. Numa era medieval sombria, você escolhe um povo, leva exércitos para a guerra e decide o que fazer com as aldeias que conquista.

> **Aviso:** o jogo tem violência explícita, e esta página mostra uma cena de morte com muito sangue.

> **Estado:** em desenvolvimento. O mapa e as aldeias são desenhados à mão, e a história está sendo escrita. Esta página é só uma apresentação: o jogo ainda não está disponível para baixar, e o código não está aqui.

![Soldados lutando no meio de uma aldeia goblin, sob a luz vermelha do clima de guerra](imagens/batalha.png)

*Ataque a uma aldeia goblin. A tela avermelha enquanto durar a guerra.*

## Quatro povos, um pacto

- **Humanos, orcs, elfos e goblins**, com homens e mulheres, civis, soldados, chefe, falas e construções próprias.
- **Sub-aldeias e aldeia principal:** a principal guarda o chefe, com soldados mais fortes e portões trancados. Para chegar lá, é preciso conquistar antes as sub-aldeias daquele povo.
- **Pacto:** você fecha em uma sub-aldeia, e ele vale para o povo inteiro, inclusive o chefe. Antes dele, ninguém te ataca, mas nenhuma porta de aldeia abre para você. Depois, os outros povos viram inimigos.
- **Rivais:** as aldeias inimigas ficam mais fortes com os dias.
- **NPCs:** andam por rotas, conversam entre si e reagem ao que acontece.

## A guerra

Cada povo chama o exército do seu jeito:

| Povo | Chamado |
|---|---|
| Humanos | Sino |
| Orcs | Trombeta |
| Elfos | Harpa |
| Goblins | Saco de moedas chacoalhado |

- **Campanha:** os soldados marcham em formação atrás de você, desviam de obstáculos e lutam ao seu lado. Você pode dispensá-los quando quiser.
- **Ponto de volta:** convocar salva o jogo. Se morrer na guerra, você volta ao lado do chamado, com tudo como estava.
- **Clima de guerra:** na aldeia atacada entram tambores, cinza e fumaça, e a área pisca em vermelho no chão e no minimapa.
- **Civis:** a maioria corre para dentro das casas, e alguns ficam do lado de fora.
- **Conquista:** quando os soldados acabam, a aldeia é sua, e os civis saem tristes e com medo. Em cada casa você pode entrar, roubar ou queimar. Queimar empobrece a aldeia.

### As defesas

- **Torres de vigia** tocam o alarme, e todos os soldados da aldeia vêm atrás de você.
- **Torres de arqueiros** também atiram flechas, que dá para desviar.
- **Portões** abrem para os soldados saírem, se trancam sozinhos se você chegar perto e reabrem para eles voltarem quando você foge.

![Personagem encapuzado entre uma oca e uma casa em chamas](imagens/fogo.png)

*Casas queimadas depois da conquista.*

## Combate e morte

O combate é em tempo real, com desmembramento conforme a vida cai: sangue vermelho, sangue verde nos zumbis e poeira nos esqueletos. Esqueleto, zumbi, lobo, vaca, galinha, veado e corvo têm sons e comportamento próprios.

Morrer tem cena própria, conforme quem te matou:

| Assassino | Cena |
|---|---|
| Esqueleto | Arranca seus órgãos, com risada sádica |
| Zumbi | Te come |
| Lobo | Te dilacera e uiva |
| Humano | Uma espadada só |
| Orc | Clava na cabeça |
| Goblins | Vários te furando sem parar |
| Elfo | Flechas, estocada e corte na garganta |

![Quatro quadros da cena de morte do elfo, com o herói caído, flechas cravadas e muito sangue](imagens/morte_elfo.png)

*Quatro momentos da cena de morte do elfo.*

## Viver no mundo

- **Mapa:** 1920 x 1440 tiles, com relevo, água, estradas e árvores que balançam com o vento.
- **Biomas:** campo, floresta, deserto e montanha, cada um com seus sons.
- **Tempo:** um dia dura 35 minutos reais, com sol, sombras e luzes noturnas.
- **Câmera:** gira de 90 em 90 graus, com minimapa e névoa de exploração.
- **Fome e descanso:** do fim da tarde até a noite dá para dormir na fogueira, o que salva o jogo e pula para o dia seguinte.
- **Itens:** inventário, armaduras, amuletos, mochilas, baús e criação de itens.
- **Barracas:** compra-se com moedas nas aldeias que não são inimigas, e rouba-se de graça durante um ataque ou depois da conquista.
- **Interiores 3D:** casas, ocas, salões e uma padaria. O sobrado e a torre élfica têm segundo andar.
- **Escritos:** livros e pergaminhos em pedaços, para juntar aos poucos.

### Três dificuldades

- **Relaxante:** ninguém briga, só você pode. Não tem fome e você entra onde quiser.
- **Normal:** o jogo como ele é.
- **Difícil:** ao morrer, seus itens ficam no chão por 3 dias. A fome é mais rápida, e as aldeias rivais sobem de nível mais rápido.

![Interior 3D da padaria, com forno, balcão e mesas com pão](imagens/padaria.png)

*A padaria por dentro.*

## O editor dentro do jogo

O mapa é feito no próprio jogo. Basta clicar em qualquer coisa para ver as opções dela. Dá para pintar o terreno, mudar o relevo, arrastar muros em linha reta, demarcar biomas e aldeias e definir as rotas dos NPCs. O teste começa em qualquer ponto do mapa.

![Editor de mapa com um NPC selecionado, seu raio de caminhada no chão e as opções no painel à direita](imagens/editor.png)

*Um NPC selecionado no editor, com o raio de caminhada no chão.*

## A história

### O que já está no jogo

No universo vazio, uma deusa branca aparece e cria a Terra. O Sol vaga ao fundo, ela o alcança e põe a Terra em órbita. Do fundo do vazio, um ser escuro e menor a observa.

Depois, na escuridão, uma voz suave chama:

> *"Oii... Olá? Tá tudo bem? Você morreu? Acorda..."*

Seus olhos abrem devagar, você vê o céu e uma mulher em silhueta contra o sol:

> *"Ah, você tá vivo... Quem é você?"*

### O que está planejado

O conflito central opõe duas grandes civilizações, e nenhuma delas é boa ou má.

| | **Ordem da Aliança** | **Confederação do Sopro** |
|---|---|---|
| Divindade | Um Deus supremo e transcendente | Muitas entidades espirituais |
| Universo | Criação com propósito | Cosmos vivo e interligado |
| Moral | Lei sagrada e justiça | Reciprocidade e equilíbrio |
| Sociedade | Centralizada, com sacerdotes e tribunais | Clãs, aldeias e conselhos de anciãos |
| Virtude | Unidade e estabilidade | Pluralidade e pertencimento |
| Perigo | Autoritarismo religioso | Fragmentação e intolerância |

Também haverá povos independentes, com histórias próprias: os Povos do Rio Ancestral, os Reinos das Máscaras e os Guardiões das Montanhas, estes com registros de eras anteriores.

Quem segue a Ordem primeiro recebe proteção e prestígio, até descobrir um segredo que compromete os governantes. O conselho então decide eliminar o protagonista. A traição é de alguns líderes, não da fé nem do povo, e sacerdotes e fiéis contrários ao conselho podem ajudar.

> **É possível construir uma ordem universal sem destruir a pluralidade dos povos, ou preservar essa pluralidade exige aceitar um mundo permanentemente dividido?**

## O que ainda vem

- Missões e a história principal.
- As aldeias e os personagens no mapa.
- Recompensas maiores por derrubar um chefe ou um povo inteiro.
- A ideia é virar um MMORPG com história, mas ainda não há rede nem servidor.

## Como é feito

Feito em Godot 4.4. Os personagens principais e as árvores partem de pranchas desenhadas pelo autor, e o resto da arte é gerado por código. Músicas e efeitos também são gerados por código, junto com gravações de domínio público ou CC0.
