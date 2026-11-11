# Pixel Sandbox

RPG de mundo aberto em pixel art, com personagens em 2D dentro de um mundo em 3D (estilo HD-2D), feito em **Godot 4.4**. O clima é de era medieval sombria: você explora, escolhe um povo, leva exércitos para a guerra e conquista ou destrói aldeias.

> **Aviso:** o jogo tem violência explícita, com desmembramento e cenas de morte com muito sangue.

> **Estado:** em desenvolvimento. O mapa e as aldeias são desenhados à mão no editor do próprio jogo, e a história ainda está sendo escrita. Esta página é só uma apresentação: o jogo ainda não está disponível para baixar, e o código não está aqui. O que já funciona está separado do que ainda é plano.

![Batalha numa aldeia](imagens/batalha.png)

## Controles

| Tecla | Ação |
|---|---|
| WASD ou setas | Andar |
| Shift | Correr (gasta fôlego) |
| Clique ou F | Bater, usar a ferramenta ou o item da mão; dentro de masmorra, atacar |
| E | Conversar, entrar, pegar, usar, comprar |
| Tab ou I | Inventário e criar itens |
| 1 a 5 | Hotbar |
| J | Caderno: anotações, bestiário, suas notas e povos |
| Z e X, ou botão do meio arrastando | Girar a câmera |
| Roda do mouse | Aproximar ou afastar |
| Esc | Pausa, salvar, configurações |

### Interface
Uma interface de RPG clássico, em molduras de couro e ouro:
- **Canto superior esquerdo:** o retrato do personagem com as barras de **PV** (com o número, e a barra acende quando a vida está baixa), **FÔL** (fôlego, que escurece quando você se esgota), **FOM** (fome) e **FRI** (frio, só aparece quando você está com frio). Embaixo, o botão do caderno, que mostra quantos escritos novos você ainda não leu.
- **Canto superior direito:** o selo do dia, com o dia em algarismos romanos, a estação e a **fase da lua**, e ao lado o minimapa redondo. Embaixo do minimapa ficam a seta do vento e o nome do bioma.
- **Embaixo:** a hotbar de cinco espaços numerados, com o nome do item que você escolheu.

## O que já existe no jogo

### Mundo
- Mapa fixo de **1920 x 1440 tiles**, com terreno 3D, relevo, água, estradas e árvores que balançam com o vento.
- Biomas de campo, floresta, deserto e montanha, cada um com seus sons e aviso ao entrar.
- Ciclo de dia e noite: um dia dura 35 minutos reais, com sol, sombras e luzes noturnas.
- Câmera que gira de 90 em 90 graus para ver tudo por todos os lados, com minimapa e névoa de exploração.

### Clima e estações
- **Vento:** tem direção de verdade e muda aos poucos. A seta num selo abaixo do minimapa mostra para onde ele sopra, e os riscos de vento, as folhas, a chuva, as nuvens e a névoa seguem essa direção.
- **Chuva:** começa sozinha, escurece o dia, molha a terra arada e traz trovão quando está forte.
- **Névoa da manhã:** aparece no fim da madrugada e some no meio da manhã. Não existe no deserto.
- **Nuvens:** ao afastar a câmera até o máximo, tufos de nuvem transparentes fecham as bordas da tela.
- **Frio:** no inverno, nas noites de outono e na montanha o corpo esfria. A barra azul de frio aparece na interface, a tela vai ficando azulada e, no limite, você perde vida. A fogueira esquenta, e o deserto nunca dá frio.

![Campo no inverno, com chão coberto de neve e árvores sem folhas](imagens/inverno.png)

*Inverno no campo.*
- **Quatro estações de 7 dias cada:**

| Estação | O que muda |
|---|---|
| Primavera | Grama verde-viva, pétalas no ar, pássaros no campo |
| Verão | Dias mais longos, poeira dourada no ar, cigarras |
| Outono | Folhas alaranjadas caindo, vento frio, noites que esfriam |
| Inverno | Neve, árvores peladas, escurece bem mais cedo, a fome aperta 35% mais, não dá para plantar e o frio machuca longe do fogo |

### Luas
A lua tem oito fases e muda a cada dia do jogo, em ciclos de oito dias: lua nova, crescente, quarto crescente, gibosa crescente, **cheia**, gibosa minguante, quarto minguante e minguante. A fase atual aparece no selo do dia.

| Fase | O que muda à noite |
|---|---|
| Lua nova | A noite é a mais escura, e os bichos hostis enxergam pouco: dá para passar por perto sem ser notado |
| Fases do meio | Aos poucos a noite clareia ou escurece |
| Lua cheia | A noite fica clara, os bichos hostis enxergam bem mais longe, os lobos uivam com mais frequência e há uivos até no campo |

Ao anoitecer numa lua cheia ou nova, um aviso conta o que esperar. Dormir pula para o dia seguinte e, portanto, para a próxima fase.

### Povos e aldeias
- **Seis povos:** humanos, orcs, elfos, goblins, **anões** e **gigantes**, cada um com homens e mulheres, civis, soldados, chefe, falas e construções próprias.
- **Anões:** baixos, barbudos e obcecados por ferro. Vivem em cavernas com abertura nas montanhas, têm forja, salão e a melhor defesa do jogo. Convocam o exército batendo a bigorna de guerra.
- **Gigantes:** têm o dobro da altura de um humano, moram em casas de lajes de pedra em pé e são os mais fortes e mais lentos. Convocam o exército com o tambor de guerra.
- **Sub-aldeias e aldeia principal:** a principal guarda o chefe, com soldados mais fortes e portões trancados. Para chegar lá, é preciso conquistar antes as sub-aldeias daquele povo.
- **Pacto:** você fecha pacto em uma sub-aldeia, e ele vale para o povo inteiro, inclusive o chefe. Antes do pacto, ninguém te ataca, mas nenhuma porta de aldeia abre para você. Depois, os outros povos viram inimigos.
- **Níveis:** as aldeias rivais ficam mais fortes com os dias. As do seu povo só vão subir com missões, que ainda serão criadas.

### Reputação com cada povo
Cada povo guarda uma opinião sobre você, de −100 a 100. Ela aparece na aba **Povos** do caderno (J), e um aviso surge quando a relação muda de faixa.

| O que você faz | Efeito |
|---|---|
| Conversar com um civil (primeira vez no dia, por povo) | +2 |
| Comprar numa barraca | +1 |
| Fechar pacto | +60 |
| Roubar de barraca abandonada | −3 |
| Matar um soldado | −4 |
| Matar um civil | −10 |
| Roubar uma casa | −10 |
| Queimar uma casa | −20 |
| Conquistar uma aldeia | −30 |

- **Amistosa (40 ou mais):** as barracas daquele povo vendem 20% mais barato, os civis te recebem bem e liberam uma pergunta extra na conversa.
- **Neutra:** tudo normal.
- **Hostil (−40 ou menos):** as barracas não vendem, os civis não conversam e recuam quando você chega perto.

### Vida dos NPCs
- **Rotina:** os civis de aldeia andam e conversam de dia. Quando anoitece ou a chuva aperta, vão até a porta mais próxima e entram; saem de manhã.
- **Reação a você:** cumprimentam quando você chega perto, com fala diferente de manhã, na chuva e conforme a reputação. Se você estiver de espada ou arco na mão, recuam e pedem para guardar.
- **Conversas com opções:** os civis dos seis povos têm um menu de perguntas (quem é o povo, que lugar é este, novidades). A novidade muda na segunda vez que você pergunta, e eles lembram que já te conheceram.
- **Personagens dentro das casas:** interiores podem ter gente lá dentro, com falas em balão, conversa e animação própria.
- Personagens importantes da história podem ser marcados: eles se escondem na guerra e não morrem.

### Guerra
- **Convocação:** cada povo chama o exército do seu jeito: **sino** (humanos), **trombeta** (orcs), **harpa** (elfos), **saco de moedas** chacoalhado (goblins), **bigorna** (anões) e **tambor** (gigantes).
- **Exército:** os soldados marcham em formação atrás de você, desviam de obstáculos e lutam com o inimigo. Você luta junto e pode dispensá-los quando quiser.
- **Ponto de volta:** convocar salva o jogo. Se morrer na guerra, você volta ao lado do chamado, com tudo como estava.
- **Clima de guerra:** ao pisar na aldeia atacada, a tela fica avermelhada, entram tambores, cinza e fumaça, e a área pisca em vermelho no chão e no minimapa.
- **Civis:** a maioria corre para dentro das casas, e alguns ficam do lado de fora.
- **Conquista:** quando os soldados acabam, a aldeia é sua. Os civis saem das casas, tristes e com medo. Você pode entrar, **roubar** ou **queimar** cada casa, e queimar empobrece a aldeia.

### Defesas
- **Torres de vigia:** veem você e tocam o alarme, e todos os soldados da aldeia vêm atrás.
- **Torres de arqueiros:** dão o alarme e atiram flechas que dá para desviar.
- **Portões:** abrem para os soldados saírem, se trancam sozinhos se você chegar perto e reabrem para eles voltarem quando você foge.
- **Perseguição:** cada soldado tem um limite de distância, ajustável no editor. Se você fugir para longe, eles voltam ao posto.

![Casas queimando](imagens/fogo.png)

### Combate e criaturas
- Combate em tempo real, com golpes, atordoamento e barras de vida.
- **Armas na mão:** espada, machado, picareta, enxada, vara de pesca e arco aparecem na mão do personagem, andando e correndo.
- **Bichos:** esqueleto, zumbi, lobo, vaca, galinha, veado, corvo e sapo, cada um com seus sons e seu jeito de agir.
- **Gore:** desmembramento conforme a vida cai, sangue vermelho, sangue verde nos zumbis, poeira nos esqueletos e pedaços pelo chão.
- **O corvo:** matar o primeiro corvo do jogo dispara um presságio: o herói de costas, relâmpagos no horizonte e um trovão. Só acontece uma vez.
- **Cena de morte para cada assassino:**
  - **Esqueleto:** arranca seus órgãos, com risada sádica.
  - **Zumbi:** te come.
  - **Lobo:** te dilacera e uiva.
  - **Humano:** uma espadada só.
  - **Orc:** clava na cabeça.
  - **Goblins:** vários te furando sem parar.
  - **Elfo:** flechas, estocada e corte na garganta.
  - **Anão:** uma picaretada na barriga que atravessa e sai nas costas.
  - **Gigante:** te ergue, te rasga em dois e joga as metades no chão.

![Cena de morte do elfo](imagens/morte_elfo.png)

### Masmorras e cavernas
- **Masmorra:** a entrada leva a três salas ligadas por escada, com esqueletos e zumbis. Clique ataca, e uma barra de vida aparece no canto. A escada e o baú só liberam com a sala limpa. O baú do fundo dá moedas, poção, ferro negro, cristal e itens sorteados, uma vez por entrada. Morrer lá dentro toca a cena de morte do bicho que matou.
- **Caverna:** uma boca na rocha que leva a uma caverna escura, com estalagmites.
- **Caverna dos anões:** a porta talhada leva à caverna onde eles vivem, com forja, bigorna, lingotes e os anões trabalhando.

### Minérios e armaduras
- **Seis minérios:** ferro, carvão, cristal, ferro negro, cobre e enxofre. As rochas de minério só quebram com picareta.
- **Armaduras de metal:** cobre (+3 de defesa), ferro (+4) e **ferro negro (+7, a melhor)**. Cada uma pede o minério e a armadura do nível anterior.
- **Barraca de ferro dos anões:** vende minério mais barato que as outras, carvão, ferramentas e as três armaduras.

### Cultivo
- **Arar:** com a enxada, a terra vira canteiro de verdade, e canteiros vizinhos se emendam numa plantação.
- **Água:** só se planta a até 8 tiles de água. Terra arada longe da água seca em um minuto. Deserto e montanha são pedra e areia, não solo.
- **Plantas:** rabanete (3 dias), nabo (4), beterraba (5), trigo (6) e maconha (7). Fumar a maconha deixa a tela rosa e ondulando, e depois você apaga e acorda no outro dia.
- **Inverno:** nada se planta, e o que estiver plantado morre de frio.

![Canteiro com rabanete, nabo, beterraba, trigo e maconha em várias fases](imagens/cultivo.png)

*Cada linha uma planta, da semente até a colheita.*

Mirtilo-branco, lírio-da-geada e cogumelo-lume nascem sozinhos no campo e na floresta, só no inverno, e brilham no escuro enquanto têm fruto. Depois de colhidos, voltam a dar fruto em dois dias. Às vezes vem uma muda, que pode ser plantada em outro lugar. Quando o inverno acaba, todos secam.

![Três plantas brilhando à noite na neve: uma moita de bolinhas brancas, um lírio azul e cogumelos claros](imagens/plantas_inverno.png)

*As plantas do inverno à noite.*

### Ferramentas e pesca
- **Do chão:** galhos e pedras pequenas aparecem pelo campo e pela floresta e mudam de lugar a cada dia. Árvores derrubadas soltam galhos, e rochas quebradas soltam pedras.
- **Improvisadas:** espada, machado e picareta de pedra amarrada num galho.
- **De ferro:** as mesmas, mais fortes. O minério vem das rochas de ferro, quebradas com picareta, ou das barracas.
- **Na mão:** a ferramenta aparece segurada o tempo todo, e cada uma tem o seu golpe. O machado derruba árvores mais rápido, a picareta quebra rochas mais rápido e a espada aumenta o dano.
- **Arco:** atira flechas no bicho mais perto, de longe.
- **Pesca:** de frente para a água, você lança a linha e a boia fica boiando. Quando o peixe morde, aparece "CLIQUE!" e, depois de fisgar, "CLIQUE RÁPIDO!" para puxar até o peixe pular para fora da água.

![Personagem na beira da água puxando um peixe, que pula para fora entre respingos](imagens/pesca.png)

*O peixe saindo da água.*

### Vida no mundo
- **Dificuldades:**
  - **Relaxante:** ninguém briga, só você pode. Não tem fome e você entra onde quiser.
  - **Normal:** o jogo como ele é.
  - **Difícil:** ao morrer, seus itens ficam no chão por 3 dias; a fome é mais rápida e as aldeias rivais sobem de nível mais rápido.
- **Fome e descanso:** a fome vai baixando com o tempo, e comida como maçã e pão alimenta. Do fim da tarde até a noite dá para dormir na fogueira, o que salva o jogo e pula para o dia seguinte.
- **Inventário e craft:** itens, armaduras, amuletos, mochilas, baús e receitas de criar itens no próprio inventário.
- **Barracas e moedas:** dá para comprar em aldeias que não são inimigas e roubar de graça durante um ataque ou depois da conquista. Dentro da padaria, o balcão também vende.
- **Interiores 3D:** casas, ocas, salões e uma padaria, cada um por dentro. O sobrado e a torre élfica têm segundo andar.
- **Escritos fragmentados:** livros e pergaminhos espalhados que você junta aos poucos.

![Interior da padaria](imagens/padaria.png)

### Editor de mapa
O jogo tem um editor completo, aberto pelo menu inicial:
- **Clicar para editar:** clique em qualquer coisa no mapa e as opções dela aparecem ao lado.
- **Ferramentas:** pintar terreno, mudar o relevo, colocar objetos com busca e categorias, e arrastar muros em linha reta.
- **Áreas:** demarcar biomas e aldeias dos seis povos, com um resumo do que falta em cada aldeia.
- **NPCs:** definir raio, rotas e distância de perseguição.
- **Objetos novos na categoria Mundo:** rochas de minério, entrada de caverna, caverna dos anões e entrada de masmorra.
- **Teste:** o F5 abre o mapa para clicar onde nascer, e o F1 abre um painel com aldeias prontas, guerra, hora, itens, cenas de morte e o presságio do corvo.

![Editor de mapa](imagens/editor.png)

## A história

### O que já está no jogo
**A abertura.** No universo vazio, uma deusa branca aparece e cria a Terra. O Sol vaga ao fundo, ela o alcança e põe a Terra em órbita. Do fundo do vazio, um ser escuro e menor a observa.

**O despertar.** Na escuridão, uma voz suave chama: *"Oii... Olá? Tá tudo bem? Você morreu? Acorda..."* Seus olhos abrem devagar, você vê o céu e uma mulher em silhueta contra o sol: *"Ah, você tá vivo... Quem é você?"* Você se levanta tonto, no mundo aberto.

**A Letícia e a padaria.** Ao acordar, a Letícia está ao seu lado. Ela te convida para a aldeia e vai andando com você até a padaria onde trabalha. Lá dentro, um eremita de um olho só está sentado sozinho num canto; Seu João e Shileno trocam murros discutindo o gosto do Seu João por mecânica; e numa mesa bebem dois orcs, um goblin e um anão, todos exilados dos seus povos por causa da bebida.

**O eremita.** Ele fala dos que foram enterrados de mau jeito e se levantam quando o sol se esconde, e avisa para estar sob um teto, perto do fogo, quando a luz for embora. Pede que você não toque nos corvos. Depois sai da padaria e some. A Letícia vem do balcão e pergunta com quem você estava falando. Ela não viu velho nenhum. Então te ensina a comprar ali mesmo.

Para essa cena acontecer, o mapa precisa ter uma padaria: a cena vale para qualquer uma colocada pelo editor.

**Os escritos.** Três textos de rascunho já podem ser coletados em pedaços: a *Crônica da Luz*, sobre a criação; *O Observador*, um aviso sobre o ser que aprendeu a desfazer o que ela fez; e *Cartas de um Soldado*, sobre a guerra vista de baixo.

### O que está planejado
O conflito central opõe duas grandes civilizações, e nenhuma delas é boa ou má:

| | **Ordem da Aliança** | **Confederação do Sopro** |
|---|---|---|
| Divindade | Um Deus supremo e transcendente | Muitas entidades espirituais |
| Universo | Criação com propósito | Cosmos vivo e interligado |
| Moral | Lei sagrada e justiça | Reciprocidade e equilíbrio |
| Sociedade | Centralizada, com sacerdotes e tribunais | Clãs, aldeias e conselhos de anciãos |
| Virtude | Unidade e estabilidade | Pluralidade e pertencimento |
| Perigo | Autoritarismo religioso | Fragmentação e intolerância |

Também haverá povos independentes, com histórias e conflitos próprios: os **Povos do Rio Ancestral**, os **Reinos das Máscaras** e os **Guardiões das Montanhas**, estes últimos com registros de eras anteriores.

Quem segue a Ordem primeiro recebe proteção e prestígio, até descobrir um segredo que compromete os governantes. O conselho então decide eliminar o protagonista. A traição é de alguns líderes, não da fé nem do povo, e sacerdotes e fiéis contrários ao conselho podem ajudar.

A pergunta que guia a história é:

> **É possível construir uma ordem universal sem destruir a pluralidade dos povos, ou preservar essa pluralidade exige aceitar um mundo permanentemente dividido?**

### Próximos passos
- Missões e a história principal.
- Colocar as aldeias, as cavernas, as masmorras e os minérios no mapa.
- Armadilhas e variedade nas masmorras.
- Recompensas maiores por derrubar um chefe ou um povo inteiro.
- Definir a parte online: a ideia é um MMORPG com história, mas ainda não há rede nem servidor.

## Como é feito

- **Motor:** Godot 4.4, em GDScript. A lógica é em 2D e a imagem é montada em 3D.
- **Arte:** os personagens principais e as árvores partem de pranchas desenhadas pelo autor. O resto é gerado por scripts em Python, em `tools/`.
- **Som:** músicas e efeitos gerados por código, mais gravações de domínio público ou CC0.
- **Créditos:** as gravações usadas são de domínio público ou CC0, e os autores estão creditados dentro do projeto.
