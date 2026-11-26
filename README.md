# Hockey — AI, 2P Local & Multiplayer Online

Jogo arcade de **Air Hockey** desenvolvido com **HTML5 Canvas**, **Tailwind CSS** e **JavaScript (ES6+)**, contando com física 2D de transferência de impulso, inteligência artificial com três níveis de dificuldade, modo duelo frente a frente no mesmo aparelho (**2P Local**) e multiplayer online P2P em tempo real via **PeerJS (WebRTC)**.

---

## Funcionalidades Principais

- **Modo vs. Inteligência Artificial:** Três níveis de dificuldade (**Fácil**, **Médio** e **Difícil**) com variação de velocidade de reação, margem de erro e antecipação de rebotes nas bordas.
- **Modo 2P Local (Frente a Frente):** Duelo no mesmo dispositivo sem necessidade de internet, com suporte a **multi-touch simultâneo** no celular/tablet (cada jogador controla sua metade da mesa) e placar invertido em 180° no topo para leitura frente a frente.
- **Modo Multiplayer Online (P2P via PeerJS):** Criação de salas privadas com código único de 5 caracteres e sincronização direta a **60 Hz** via WebRTC DataChannel, sem necessidade de backend próprio ou configuração de banco de dados.
- **Responsividade Inteligente (Portrait & Landscape):** Em smartphones na orientação retrato, a mesa gira automaticamente para o eixo vertical para controle ergonômico com o polegar e o HUD reorganiza o placar e a etiqueta de modo em duas faixas; em desktops e tablets, exibe a mesa panorâmica horizontal.
- **Física 2D Realista:** Transferência vetorial de velocidade nas tacadas (*smash*), atrito simulado de mesa de ar, rastro luminoso no disco, partículas de impacto e leve vibração de tela (*screen shake*).
- **Áudio Sintetizado:** Efeitos sonoros de impacto, tabela, contagem regressiva e gol gerados dinamicamente via **Web Audio API**, sem dependência de arquivos externos.

---

## Estrutura de Arquivos

```text
hockey-game/
├── index.html   # Aplicação completa: estrutura semântica, HUD responsivo, estilos neon, física 2D, IA, Web Audio API e rede P2P (PeerJS)
└── README.md    # Documentação do projeto