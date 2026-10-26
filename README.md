# NZXT Kraken 360 LCD (RL-KR360-B1) - Web Integration

Tema customizado para o display LCD do water cooler NZXT Kraken 360 (RL-KR360-B1) utilizando o modo Web Integration do NZXT CAM.

## Especificações do Hardware
- **Modelo:** NZXT Kraken 360 RGB (RL-KR360-B1)
- **Tela:** 1.54" TFT (240 x 240 pixels)
- **Taxa de Atualizacao:** 30 Hz

## Como testar localmente

1. Abra o terminal na pasta do projeto (`D:\Projetos\nzxt-kraken-lcd`):
   ```bash
   python -m http.server 3000
   ```
2. No seu navegador, acesse `http://localhost:3000` para ver o preview com dados simulados (Mock Preview).
3. No software NZXT CAM:
   - Vá na aba **LCD Display** -> **Web Integration**.
   - Selecione **Custom Web Integration**.
   - Clique em **Configure**.
   - Insira o endereço `http://localhost:3000`.
   - Salve as alterações.

## Publicando no GitHub Pages (Sem precisar de servidor local)

Para não precisar manter um terminal ou servidor web rodando na sua máquina:
1. Crie o repositório `nzxt-kraken-lcd` no seu GitHub (`https://github.com/new`).
2. Suba o código para a branch `main`.
3. Vá em **Settings** -> **Pages** no GitHub e selecione a branch `main` (pasta `/root`).
4. Copie a URL gerada (exemplo: `https://tioeddie-hub.github.io/nzxt-kraken-lcd/`) e coloque diretamente no NZXT CAM.