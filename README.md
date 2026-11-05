# Lembretes

Aplicativo web em português para criar e acompanhar lembretes com título, descrição opcional, data e horário. A interface permite alternar entre lembretes pendentes e concluídos, editar ou excluir itens e ajustar aparência, texto, lista e notificações nas configurações.

O projeto também inclui recursos de PWA: pode ser instalado pelo navegador e tem suporte a cache para uso offline.

## Como executar

Os arquivos fornecidos não incluem instruções de instalação, dependências ou processo de build. Para usar os recursos de PWA, publique os arquivos em um servidor com HTTPS. O service worker só é registrado quando o app é aberto por HTTP ou HTTPS.

## Arquivos

- `index.html` — interface e lógica do aplicativo.
- `manifest.webmanifest` — metadados para instalação como PWA.
- `sw.js` — cache para uso offline e tratamento de cliques em notificações.
- `apple-touch-icon.png`, `badge-96.png`, `icon-192.png`, `icon-512.png`, `maskable-512.png` — imagens do aplicativo.

## Observação

No código, os ícones são referenciados dentro de uma pasta `icons/`, mas no ZIP fornecido estão na raiz. Para que esses ícones sejam carregados, coloque-os em `icons/` ou ajuste os caminhos em `index.html`, `manifest.webmanifest` e `sw.js`.
