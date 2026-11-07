# Pixel Sandbox

RPG de mundo aberto em pixel art, com personagens em 2D dentro de um mundo em 3D. Numa era medieval sombria, você escolhe um povo, leva exércitos para a guerra, planta, pesca, enfrenta o frio do inverno e decide o que fazer com as aldeias que conquista.

> **Aviso:** o jogo tem violência explícita, e esta página mostra uma cena de morte com muito sangue.

> **Estado:** em desenvolvimento. O mapa e as aldeias são desenhados à mão, e a história está sendo escrita. Esta página é só uma apresentação: o jogo ainda não está disponível para baixar, e o código não está aqui.

![Soldados lutando no meio de uma aldeia goblin, sob a luz vermelha do clima de guerra](imagens/batalha.png)

*Ataque a uma aldeia goblin. A tela avermelha enquanto durar a guerra.*

## Controles

| Tecla | Ação |
|---|---|
| WASD ou setas | Andar |
| Shift | Correr |
| Clique ou F | Usar o que está na mão: bater, cortar, arar, plantar, pescar |
| E | Conversar, entrar, pegar, colher |
| 1 a 5 | Escolher o que fica na mão |
| Tab ou I | Inventário, equipamento e criar itens |
| J | Caderno |
| Z e X | Girar a câmera |
| Roda do mouse | Aproximar ou afastar |
| Esc | Pausa |

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

O combate é em tempo real, com desmembramento conforme a vida cai: sangue vermelho, sangue verde nos zumbis e poeira nos esqueletos. Esqueleto, zumbi, lobo, vaca, galinha, veado e corvo têm sons e comportamento próprios. Com uma espada na mão, o dano sobe.

Morrer tem cena própria, conforme quem te matou:

| Assassino | Cena |
|---|---|
| Esqueleto | Arranca seus órgãos, com risada sádica |
| Zumbi | Te come |
| Lobo | Te dilacera e uiva |
| Humano | Uma espadada arranca a cabeça; o corpo fica de pé jorrando, ajoelha e tomba |
| Orc | A clava esmaga a cabeça, joga o corpo de costas e abre a barriga |
| Goblins | Furam as pernas até você cair de joelhos, e você morre ajoelhado |
| Elfo | Flechas te pregam numa árvore, e você morre de pé |

![Quatro quadros da cena de morte do elfo: o herói pregado numa árvore por flechas, a estocada e o corte na garganta](imagens/morte_elfo.png)

*A cena de morte do elfo.*

## Estações do ano

Primavera, verão, outono e inverno, com 7 dias cada, em todos os biomas menos o deserto. A mudança é dia a dia: no outono as copas ficam alaranjadas e as folhas caem, no inverno a neve cobre o chão e as árvores ficam peladas, e na primavera a neve derrete em manchas até a grama voltar.

![Campo no inverno, com chão coberto de neve e árvores sem folhas](imagens/inverno.png)

*Inverno no campo.*

### Frio

No inverno, nas noites de outono e na montanha, o corpo esfria. Uma barra azul aparece embaixo da fome, a tela vai ficando azulada e, no limite, você perde vida. A fogueira esquenta, e o deserto nunca dá frio.

## Cultivo

- **Arar:** com a enxada, a terra vira canteiro de verdade, e canteiros vizinhos se emendam numa plantação.
- **Água:** só se planta a até 8 tiles de água. Terra arada longe da água seca em um minuto. Deserto e montanha são pedra e areia, não solo.
- **Plantas:** rabanete (3 dias), nabo (4), beterraba (5), trigo (6) e maconha (7). Fumar a maconha deixa a tela rosa e ondulando, e depois você apaga e acorda no outro dia.
- **Inverno:** nada se planta, e o que estiver plantado morre de frio.

![Canteiro com rabanete, nabo, beterraba, trigo e maconha em várias fases](imagens/cultivo.png)

*Cada linha uma planta, da semente até a colheita.*

### Plantas do inverno

Mirtilo-branco, lírio-da-geada e cogumelo-lume nascem sozinhos no campo e na floresta, só no inverno, e brilham no escuro enquanto têm fruto. Depois de colhidos, voltam a dar fruto em dois dias. Às vezes vem uma muda, que pode ser plantada em outro lugar. Quando o inverno acaba, todos secam.

![Três plantas brilhando à noite na neve: uma moita de bolinhas brancas, um lírio azul e cogumelos claros](imagens/plantas_inverno.png)

*As plantas do inverno à noite.*

## Ferramentas e pesca

- **Do chão:** galhos e pedras pequenas aparecem pelo campo e pela floresta e mudam de lugar a cada dia. Árvores derrubadas soltam galhos, e rochas quebradas soltam pedras. Itens caídos flutuam e ganham borda amarela quando você chega perto.
- **Improvisadas:** espada, machado e picareta de pedra amarrada num galho.
- **De ferro:** as mesmas, mais fortes. O minério vem das rochas de ferro da montanha, quebradas com picareta, ou das barracas, e custa caro.
- **Na mão:** a ferramenta aparece segurada o tempo todo, e cada uma tem o seu golpe. O machado derruba árvores mais rápido, a picareta quebra rochas mais rápido e a espada aumenta o dano.
- **Pesca:** de frente para a água, você lança a linha e a boia fica boiando. Quando o peixe morde, aparece "CLIQUE!" e, depois de fisgar, "CLIQUE RÁPIDO!" para puxar até o peixe pular para fora da água. Os peixes como item ainda vão entrar.

![Personagem na beira da água puxando um peixe, que pula para fora entre respingos](imagens/pesca.png)

*O peixe saindo da água.*

## Viver no mundo

- **Mapa:** 1920 x 1440 tiles, com relevo, água e árvores que balançam com o vento.
- **Biomas:** campo, floresta, deserto e montanha, cada um com seus sons.
- **Tempo:** um dia dura 35 minutos reais, com sol, sombras e luzes noturnas. O nome da estação aparece junto com o dia.
- **Câmera:** gira de 90 em 90 graus, com minimapa e névoa de exploração.
- **Fome e descanso:** do fim da tarde até a noite dá para dormir na fogueira, o que salva o jogo e pula para o dia seguinte.
- **Inventário:** itens são arrastados entre a mochila, a mão e o equipamento: cabeça, peito, pernas, botas, amuleto e mochila, que aumenta os espaços. Criar itens fica no próprio inventário.
- **Barracas:** compra-se com moedas nas aldeias que não são inimigas, e rouba-se de graça durante um ataque ou depois da conquista.
- **Interiores 3D:** casas, ocas, salões e uma padaria. O sobrado e a torre élfica têm segundo andar.
- **Caderno:** tudo o que você lê e ouve vai sendo anotado em ordem, e cada livro ou pergaminho mostra os trechos que ainda faltam. A história virá aos pedaços, de livros nas casas, conversas e missões.

### Três dificuldades

- **Relaxante:** ninguém briga, só você pode. Não tem fome e você entra onde quiser.
- **Normal:** o jogo como ele é.
- **Difícil:** ao morrer, seus itens ficam no chão por 3 dias. A fome é mais rápida, e as aldeias rivais sobem de nível mais rápido.

![Interior 3D da padaria, com forno, balcão e mesas com pão](imagens/padaria.png)

*A padaria por dentro.*

## O editor dentro do jogo

O mapa é feito no próprio jogo. Basta clicar em qualquer coisa para ver as opções dela. Dá para pintar o terreno, mudar o relevo, arrastar muros em linha reta, demarcar biomas e aldeias, definir as rotas dos NPCs e assistir a todas as cenas de morte. O teste começa em qualquer ponto do mapa, com um painel para pular o dia, mudar a estação, ganhar itens e montar aldeias prontas.

![Editor de mapa com a aba de cenas de morte aberta](imagens/editor.png)

*O editor, com a lista de cenas de morte.*

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
- Peixes, receitas novas e mais coisas para o frio.
- Recompensas maiores por derrubar um chefe ou um povo inteiro.
- A ideia é virar um MMORPG com história, mas ainda não há rede nem servidor.

## Como é feito

Feito em Godot 4.4. Os personagens principais e as árvores partem de pranchas desenhadas pelo autor, e o resto da arte é gerado por código. Músicas e efeitos também são gerados por código, junto com gravações de domínio público ou CC0.
