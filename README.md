# Projeto-dino-automatico


#  Bot do Jogo Dino (Google Chrome)

Este projeto é um bot em Python que joga automaticamente o jogo Dino do Google Chrome (aquele jogo do dinossauro que aparece quando está sem internet). Ele detecta obstáculos na tela e pula automaticamente usando reconhecimento de imagem com a biblioteca PyAutoGUI.

---

##  Requisitos

- Python 3.7 ou superior
- Biblioteca [PyAutoGUI](https://pyautogui.readthedocs.io/en/latest/)
- Imagens dos obstáculos na pasta `.\Automacao\img`
- Imagem do dinossauro salva como `dino.png` em `.\Automacao\`

### Instale as dependências com:

```bash
pip install pyautogui


Automacao/
├── img/
│   ├── cacto1.png
│   ├── cacto2.png
│   └── ... outras imagens de obstáculos
├── dino.png
└── bot.py
Como Usar

Abra o navegador Google Chrome.

Digite chrome://dino na barra de endereços e pressione Enter.

Coloque a janela do jogo em primeiro plano.

Execute o script Python:

python bot.py


O bot irá procurar os obstáculos na tela. Quando encontrar um obstáculo próximo do dinossauro, ele pressionará a tecla espaço para pular automaticamente.

 Como Funciona

O script percorre todas as imagens na pasta img/.

Usa pyautogui.locateOnScreen() para encontrar as imagens dos obstáculos e a posição do dinossauro na tela.

Compara a posição horizontal dos dois:

Se o obstáculo estiver a uma distância igual ou menor que 170px do dinossauro, o bot aciona o pulo (space).

 Aviso

O script depende da resolução e escala da tela. Use o jogo com zoom de 100% no navegador para melhores resultados.

Não minimize a janela do jogo – o PyAutoGUI só funciona com o que está visível na tela.

Este projeto é apenas para fins educacionais.

📄 Licença

Distribuído sob a licença MIT. Veja LICENSE para mais informações.


Autor:

Feito por [Eduardo Oliveira Silva Martins]

