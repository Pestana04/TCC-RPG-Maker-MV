# 🎮 Missão UAI

**Missão UAI** é um jogo educacional desenvolvido no **RPG Maker MV** com o objetivo de apresentar, de maneira interativa, as principais etapas envolvidas no processo de emissão de um passaporte.

O projeto foi desenvolvido como **Trabalho de Conclusão de Curso**, utilizando elementos de RPG, exploração, missões, diálogos, simulações e pequenas cenas narrativas para transformar um processo burocrático em uma experiência mais acessível e dinâmica.

---

## 📖 Sobre o jogo

A protagonista precisa emitir seu primeiro passaporte.

Para isso, o jogador deverá acompanhar toda a jornada, começando dentro do apartamento da personagem e passando por diferentes situações, até receber o passaporte em seu apartamento.

Entre as etapas estão:

- conversar com familiares;
- conseguir um cartão;
- acessar o computador;
- realizar a solicitação;
- efetuar o pagamento;
- realizar o agendamento;
- aguardar o horário marcado;
- sair de casa;
- pegar um táxi;
- localizar a UAI;
- aguardar atendimento;
- tirar a foto 3x4;
- retornar para casa;
- aguardar a emissão do documento;
- receber o passaporte.

O jogo também possui missões secundárias e pequenas situações opcionais durante a exploração.

---

# 🗺️ Ambientes

O projeto possui diferentes mapas desenvolvidos para representar a jornada da protagonista.

Entre eles:

- Apartamento da protagonista;
- Apartamento da protagonista 2;
- Lojinha;
- Corredor do prédio;
- Vizinhança;
- Cidade Vista por Cima;
- Shopping Fora;
- Shopping Dentro;
- Elevador;
- Banheiro Feminino;
- Interior do shopping;
- UAI;
- Computador virtual;
- Sala de introdução;
- Sala de tutorial.

Cada ambiente possui eventos, NPCs e interações próprias.

---

# 🎯 Sistema de Missões

O jogo utiliza um sistema de missões baseado no **Galv's Quest Log**, integrado a um plugin próprio desenvolvido para o projeto.

A missão principal acompanha todo o processo de emissão do passaporte.

Exemplo:

```text
Em Busca do Passaporte

• Converse com vovó
• Converse com sua mãe
• Pegue seu cartão
• Agende a consulta
• Espere até o horário
• Vá para fora do prédio
• Pegue o táxi
• Encontre a UAI
• Espere na fila
• Tire a foto 3x4
• Espere o atendente
• Vá para casa
• Espere seu passaporte
```

Além da missão principal, o jogo também possui conteúdo secundário.

---

# 🧭 MissaoHUD

Para facilitar o acompanhamento das missões foi desenvolvido o plugin próprio:

```text
MissaoHUD
```

Ele exibe no canto da tela:

- missão atualmente rastreada;
- objetivo atual;
- indicação de novos objetivos;
- alterações de progresso;
- aviso de missão concluída.

Exemplo:

```text
┌─────────────────────────────┐
│ MISSÃO ATUAL                │
│                             │
│ Em Busca do Passaporte      │
│ • Tire a foto 3x4           │
└─────────────────────────────┘
```

O HUD é integrado ao **Galv's Quest Log**.

---

# 🎓 TutorialHUD

Durante testes iniciais do projeto, alguns jogadores que nunca haviam utilizado jogos feitos no RPG Maker tiveram dificuldade para identificar os controles.

Para solucionar esse problema foi desenvolvido o:

```text
TutorialHUD
```

O plugin cria um tutorial interativo dentro do jogo.

Entre as etapas estão:

- movimentação;
- corrida;
- interação;
- abertura do menu;
- acesso ao sistema de missões;
- rastreamento de outra missão;
- retorno para a missão do tutorial.

O HUD também reage às teclas pressionadas pelo jogador.

Exemplo:

```text
┌─────────────────────────────┐
│ MOVIMENTAÇÃO                │
│                             │
│ Use as teclas para andar.   │
│                             │
│           ↑                 │
│        ←  ↓  →              │
└─────────────────────────────┘
```

---

# 🎮 Controles

## Movimentação

```text
↑ ↓ ← →
```

## Correr

```text
SHIFT + direção
```

## Interagir / Confirmar

```text
ENTER
ESPAÇO
Z
```

## Abrir Menu / Voltar

```text
ESC
X
```

Os controles também podem ser consultados através da opção:

```text
Menu → Controles
```

---

# 💻 Computador virtual

Uma das principais partes do jogo é a simulação do computador utilizado pela protagonista.

A interface possui:

- Área de Trabalho;
- Portal UAI;
- Solicitação;
- Pagamento;
- Agendamento;
- navegação através de botões interativos.

O computador foi desenvolvido utilizando eventos do RPG Maker MV e plugins adicionais para interação com elementos da tela.

---

# 🕐 Sistema de horário

O horário escolhido durante o processo de agendamento influencia determinados elementos do jogo.

O projeto possui variações para:

- manhã;
- tarde;
- noite.

Dependendo do horário, podem ser alterados:

- tonalidade da tela;
- NPCs presentes;
- sons ambientes;
- eventos;
- movimentação de personagens;
- elementos do cenário.

---

# 🏙️ Mundo mais dinâmico

Diversos eventos foram adicionados apenas para fazer os mapas parecerem mais vivos.

Alguns exemplos:

- veículos circulando pela cidade;
- motociclistas;
- NPCs andando pelas ruas;
- cachorro perseguindo gato;
- pessoas entrando e saindo de estabelecimentos;
- sons ambientes;
- movimentação da fila da UAI;
- pessoas desaparecendo dos balcões após serem atendidas;
- mudanças de NPCs dependendo do horário.

Esses eventos não são necessariamente obrigatórios para concluir o jogo, mas ajudam na ambientação.

---

# 🛂 UAI

A UAI representa a etapa final do processo presencial.

O jogador deverá:

```text
Chegar à UAI
      ↓
Esperar na fila
      ↓
Realizar atendimento
      ↓
Tirar foto 3x4
      ↓
Esperar o atendente
      ↓
Receber orientações
      ↓
Voltar para casa
```

Após o atendimento, a protagonista é informada de que deverá aguardar aproximadamente **14 dias** para receber o documento.

---

# 📕 Passaporte

Depois da passagem de tempo, o documento finalmente é entregue no apartamento da protagonista.

O último objetivo da missão principal é então concluído:

```text
✓ Espere seu passaporte
```

seguido da conclusão:

```text
MISSÃO CONCLUÍDA

Em Busca do Passaporte
```

---

# 🎬 Pós-créditos

O jogo possui uma pequena cena pós-créditos relacionada ao futuro da protagonista.

Agora com seu passaporte em mãos, ela começa a pesquisar possíveis destinos para uma futura viagem.

Essa cena também funciona como uma referência à possibilidade de expansão do projeto.

---

# 🛠️ Tecnologias

O projeto foi desenvolvido utilizando:

- RPG Maker MV;
- JavaScript;
- plugins da comunidade;
- plugins próprios;
- Git;
- GitHub;
- IntelliJ IDEA.

---

# 🔌 Plugins próprios

## MissaoHUD

Plugin responsável pela interface permanente de acompanhamento de missões.

Principais funcionalidades:

- integração com Galv's Quest Log;
- missão rastreada;
- objetivo atual;
- atualizações automáticas;
- mensagens de missão concluída;
- possibilidade de ocultar temporariamente a HUD.

---

## TutorialHUD

Plugin responsável pelo sistema interativo de tutorial.

Principais funcionalidades:

- instruções visuais;
- detecção de teclas;
- feedback visual;
- integração com missões;
- Quest Exemplo;
- tela de controles;
- integração com MissaoHUD.

---

# 🔌 Plugins de terceiros

O projeto utiliza plugins desenvolvidos pela comunidade RPG Maker.

Entre eles estão plugins de:

### Galv's Scripts

- Galv's Quest Log;
- Galv's Cam Control;
- Galv's Screen Buttons;
- Galv's Map Travel;
- Galv's Message Sound Effects.

Site do autor:

```text
https://galvs-scripts.com/
```

Os respectivos plugins permanecem sujeitos aos termos de uso de seus autores.

---

# 🎨 Recursos gráficos

O projeto utiliza uma combinação de:

- recursos padrões do RPG Maker MV;
- assets adquiridos legalmente;
- recursos disponibilizados pela comunidade;
- modificações gráficas realizadas para o projeto;
- imagens produzidas especificamente para o jogo;
- imagens geradas por IA generativa.

---

## Shopping Mall Tileset

Alguns ambientes do shopping utilizam recursos do:

```text
RPG Maker MV - Shopping Mall Tileset
```

Desenvolvido por:

```text
Gotcha Gotcha Games
```

Este conteúdo é um recurso comercial e permanece sujeito aos termos de licença do produto original.

---

## Street Lighting and Motorcycle Gangs

Autor:

```text
Daniel Y.R.
```

Recurso utilizado como referência/material para iluminação noturna e movimentação urbana.

---

## Free Icon Pack

Créditos:

```text
SirAndriy
```

O autor permite utilização em projetos comerciais e não comerciais, com atribuição.

---

## STV Window Skins

Créditos:

```text
SkottyTV
```

Conjunto de Window Skins disponibilizado para projetos comerciais e não comerciais.

---

# 🤖 Inteligência Artificial

O **OpenAI ChatGPT** foi utilizado como ferramenta auxiliar durante o desenvolvimento do projeto.

Seu uso incluiu:

- apoio na resolução de problemas;
- auxílio na depuração de eventos;
- discussão de soluções para RPG Maker MV;
- auxílio na estruturação dos plugins próprios;
- apoio na documentação;
- geração e edição de imagens utilizadas em cenas do jogo;
- auxílio na organização de ideias e fluxos narrativos.

As decisões de implementação, integração, testes e desenvolvimento do projeto foram realizadas pelo autor.

---

# 👨‍💻 Autor

**Gustavo Pestana**

Projeto desenvolvido como Trabalho de Conclusão de Curso.

---

# 🚀 Como executar o projeto

## Pelo RPG Maker MV

Clone o repositório:

```bash
git clone https://github.com/Pestana04/TCC---RPG-Maker-MV.git
```

Abra a pasta do projeto e execute:

```text
Game.rpgproject
```

com o **RPG Maker MV**.

---

## Versão distribuída

Caso uma versão executável esteja disponível na seção de **Releases**, basta baixá-la, extrair os arquivos e executar:

```text
Game.exe
```

---

# 📂 Estrutura simplificada

```text
Missao-UAI/
│
├── audio/
│
├── data/
│
├── fonts/
│
├── icon/
│
├── img/
│
├── js/
│   ├── libs/
│   └── plugins/
│
├── Game.rpgproject
├── index.html
├── package.json
└── README.md
```

---

# ⚠️ Aviso sobre assets

Alguns recursos utilizados no desenvolvimento possuem licenças próprias ou são conteúdos comerciais.

Por esse motivo, determinados assets podem não estar incluídos neste repositório público.

A disponibilização do código-fonte deste projeto **não concede direitos de redistribuição sobre assets de terceiros**.

Para utilizar esses recursos em outro projeto, consulte e respeite os termos de licença dos respectivos autores e produtos.

---

# 📌 Estado do projeto

O fluxo principal do jogo está implementado.

Atualmente o projeto está em fase de:

```text
Polimento
```

com foco em:

- correção de bugs;
- melhorias nos diálogos;
- ajustes de áudio;
- melhorias visuais;
- transições;
- balanceamento de eventos;
- refinamento dos NPCs;
- revisão dos créditos;
- testes completos do início ao fim.

---

# 🌎 Possibilidades futuras

A estrutura do jogo permite futuras expansões.

Entre as ideias consideradas estão:

- utilização do passaporte;
- viagens;
- novos mapas;
- novos destinos;
- novas missões;
- expansão da história da protagonista.

Uma missão conceitual já representa essa possibilidade:

```text
Viajar o Mundo
```

---

# 📄 Direitos e licenças

O código desenvolvido especificamente para **Missão UAI** pertence ao autor do projeto.

Plugins, tilesets, imagens, músicas, efeitos sonoros e demais conteúdos de terceiros continuam sujeitos às licenças de seus respectivos criadores.

Consulte os créditos e termos de cada recurso antes de reutilizá-los em outros projetos.

---

# ❤️ Agradecimentos

Um agradecimento especial à minha irmã Julia que me ajudou durante os testes do jogo, minha vó Isabel que serviu de inspiração para fazer a "Vó" do jogo, meu pai pelo seu suporte e ao meu orientador do projeto Tassio Ferenzini Martins Sirqueira.
Também aos desenvolvedores da comunidade RPG Maker que disponibilizam ferramentas, plugins e recursos que possibilitaram a construção do projeto.

Em homenagem a minha querida mãe Carmen Lucia Zavon que não conseguiu me ver formando devido ao seu falecimento em 2024, fiz possível sua participação por meio da personagem "Mãe" dentro do jogo.

---

<p align="center">
  <b>Missão UAI</b><br>
  Do primeiro passo até o primeiro passaporte.
</p>
