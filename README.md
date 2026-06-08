# 🐭 Ratatoing — Fuja do Velho!

**Integrantes:** Arthur Krauze, João Vitor Simão, Pedro Henrique J

🎥 **Vídeo no YouTube:** [https://youtu.be/fP1LlS-tqv4]

---

## Sobre o Jogo

Você é um rato que precisa coletar todos os cálices espalhados pelo labirinto antes de conseguir avançar ao próximo nível — mas cuidado! Um velho furioso armado com bengala está te perseguindo. São 10 fases com labirintos cada vez mais desafiadores e o velho ficando mais rápido a cada nível.

---

## Como Executar

O jogo roda diretamente no navegador, sem necessidade de instalação ou servidor.

### Opção 1 — Abrir direto no navegador

1. Faça o download ou clone o repositório
2. Abra o arquivo `index.html` diretamente no seu navegador (Chrome, Firefox, Edge etc.)
3. Pronto! O jogo carregará automaticamente

### Opção 2 — Servidor local (recomendado para evitar erros de CORS)

Se preferir usar um servidor local, com Python instalado basta rodar:

```bash
# Python 3
python -m http.server 8000
```

Depois acesse `http://localhost:8000` no navegador.

### Dependências

Nenhuma instalação necessária. A única dependência é a biblioteca **p5.js v1.9.0**, carregada automaticamente via CDN no `index.html`.

---

## Como Jogar

| Tecla | Ação |
|---|---|
| `W` ou `↑` | Mover para cima |
| `S` ou `↓` | Mover para baixo |
| `A` ou `←` | Mover para a esquerda |
| `D` ou `→` | Mover para a direita |
| `ENTER` ou clique | Confirmar / Avançar tela |

### Objetivo

- Colete **todos os cálices** 🏆 espalhados pelo labirinto para completar a fase
- **Fuja do velho** — se ele te alcançar, você perde tudo!
- Complete os **10 níveis** para virar campeão

### Dicas

- Fique de olho na **vinheta vermelha** nas bordas da tela: quanto mais intensa, mais perto o velho está
- A tela **treme** quando o perigo é máximo — hora de correr!
- O velho usa pathfinding inteligente (BFS) e fica mais rápido a cada nível
- Planeje sua rota: colete os cálices mais distantes primeiro, enquanto o velho ainda está longe

### Pontuação

- **100 pontos** por cada cálice coletado
- A pontuação acumula entre as fases
- Se perder, a pontuação reinicia do zero

---

## Estrutura do Projeto

```
ratatoing/
├── index.html   # Página principal do jogo
├── style.css    # Estilos visuais
├── script.js    # Lógica completa do jogo (p5.js)
└── README.md    # Este arquivo
```
