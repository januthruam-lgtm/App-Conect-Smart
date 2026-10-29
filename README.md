# Smartwatch BLE

App web de arquivo único para conectar, explorar e testar comandos Bluetooth Low Energy (BLE) de smartwatches genéricos do ecossistema HryFine, usando a Web Bluetooth API.

## Requisitos
- Celular Android com Bluetooth ligado
- Google Chrome atualizado
- Página aberta via HTTPS (ex.: GitHub Pages)

## Como publicar no GitHub Pages
1. Suba o arquivo `index.html` na raiz do repositório.
2. Vá em Settings > Pages.
3. Em "Build and deployment", escolha "Deploy from a branch", branch `main`, pasta `/ (root)`.
4. Salve e aguarde o link `https://SEU-USUARIO.github.io/NOME-DO-REPO/`.

## Como usar
1. Abra o link no Chrome do celular.
2. Toque em "Buscar relógio" e escolha o dispositivo.
3. Veja os serviços e características, leia valores e ative notificações.
4. Escolha uma característica de escrita e envie bytes em HEX.
5. Use o log para mapear quais bytes fazem cada ação.

## Observações
- O Chrome só expõe serviços declarados antes da busca. Se o relógio usar UUIDs fora da lista padrão, informe em "UUIDs extras".
- Se o relógio estiver conectado ao app HryFine, desconecte lá antes, pois o BLE aceita uma conexão por vez.
- Nunca publique sua API Key do Google AI Studio no repositório.
