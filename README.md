# COBRINHA-JOGO-NO-PYTHON
Apresentado por Luan David e Ederson 
Uma implementação clássica e interativa do **Jogo da Cobrinha** desenvolvida em **Python 3** utilizando a biblioteca **Pygame**. O projeto foi estruturado utilizando conceitos de **Programação Orientada a Objetos (POO)** para garantir um código limpo, modular e de fácil manutenção.

---

## 📸 Demonstração e Visual do Jogo

- **Janela:** 500x500 pixels.
- **Estilo:** Visual minimalista em grelha com atualização em tempo real.
- **Pontuação:** Exibida dinamicamente no título da janela.

---

## 🚀 Funcionalidades

- **Movimentação Fluida:** Controlo preciso da cobra utilizando as setas do teclado.
- **Bloqueio de Inversão de Sentido:** Impede que a cobra colida instantaneamente consigo mesma ao tentar ir na direção oposta.
- **Geração Inteligente de Frutas:** As frutinhas surgem de forma aleatória sem nunca nascerem em cima do corpo da cobra.
- **Deteção de Colisão:**
  - Colisão com as bordas da tela (paredes).
  - Colisão da cabeça da cobra com o próprio corpo (auto-colisão).
  - Colisão com a frutinha para crescimento e pontuação.
- **Placar Dinâmico:** Atualização instantânea da pontuação no cabeçalho da janela a cada frutinha coletada.
- **Sistema de Reinício:** Reinicialização automática do jogo ao colidir.

---

## 🛠️ Tecnologias Utilizadas

- **[Python 3](https://www.python.org/)** — Linguagem principal do projeto.
- **[Pygame](https://www.pygame.org/)** — Biblioteca utilizada para renderização gráfica, controle de eventos e física do jogo.

---

## ⚙️ Como Executar o Projeto

### Pré-requisitos
Certifica-te de que tens o **Python 3** instalado na tua máquina.

### 1. Clonar ou Baixar o Repositório
Clona o repositório para a tua máquina local ou faz o download dos ficheiros `.zip`:
```bash
git clone [https://github.com/teu-usuario/Jogo_da_Cobrinha_Python.git](https://github.com/teu-usuario/Jogo_da_Cobrinha_Python.git)
cd Jogo_da_Cobrinha_Python
2. Instalar as DependênciasInstala a biblioteca pygame através do pip:Bashpip install pygame
3. Executar o JogoRoda o script do jogo com o comando:Bashpython snake.py
🎮 Comandos do JogoTeclaAçãoSeta para Cima (↑)Move a cobra para CimaSeta para Baixo (↓)Move a cobra para BaixoSeta para Esquerda (←)Move a cobra para a EsquerdaSeta para Direita (→)Move a cobra para a DireitaBotão Fechar (X)Encerra o jogo🧩 Estrutura do Código e ArquiteturaO código é dividido em duas classes principais que gerenciam a lógica dos elementos do jogo:1. Snake (Classe da Cobra)Atributos:cor: Definição RGB da cor da cobra.tamanho: Dimensão de cada segmento em pixels (10x10).corpo: Lista de tuplas representando as coordenadas de cada segmento.direcao: String com a direção atual ('direita', 'esquerda', 'cima', 'baixo').pontos: Contador de pontuação do jogador.Métodos Principais:andar(): Atualiza a posição do corpo movendo a cabeça na direção atual e removendo a cauda.comer(): Aumenta o tamanho do corpo adicionando um novo segmento à cauda e incrementa o placar.colisao(): Avalia se a cabeça atingiu os limites da tela ou se colidiu com a cauda.2. Frutinha (Classe da Fruta)Atributos:cor: Definição RGB (Vermelho).posicao: Tupla (x, y) gerada aleatoriamente na grelha.Métodos Principais:criar_posicao(cobrinha): Método estático que sorteia coordenadas no plano de 500x500 garantindo que a nova fruta não surja sob o corpo da cobra.📜 LicençaEste projeto está sob a licença MIT. Sinta-se livre para estudar, modificar e distribuir o código.
