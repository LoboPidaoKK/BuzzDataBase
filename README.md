# BuzzDataBase — versão 5 (IndexedDB)

Esta versão usa IndexedDB para guardar os metadados da coleção e uma store separada para as capas personalizadas. Isso evita o limite reduzido do `localStorage` que impedia importar catálogos maiores.

## Publicar no GitHub Pages

1. Extraia este ZIP.
2. Envie todos os arquivos que estão dentro dele para a raiz do repositório `BuzzDataBase`, substituindo os antigos.
3. Faça commit e aguarde o GitHub Pages publicar a atualização.
4. Abra o site atualizado e toque em **Importar backup**.
5. Escolha o arquivo `buzzdatabase-backup.json` com as 429 obras.

## Dados e backup

- A importação substitui a coleção apenas naquele navegador/dispositivo, e agora grava no IndexedDB.
- Backups antigos com `items`, `sections` e `favorites` continuam aceitos.
- As capas personalizadas são mantidas; imagens Base64 são armazenadas separadamente dos dados de título/tópico.
- A busca automática/cache automático de capas foi removida. Sem capa personalizada, o cartão exibe um símbolo.
- Na primeira abertura, a aplicação tenta migrar dados legados do localStorage; após gravar no IndexedDB com sucesso, remove as chaves antigas e o cache antigo de capas.
- Depois de importar, exporte um novo backup para conferir e guarde uma cópia fora do navegador.
- O armazenamento local continua sendo específico de cada navegador/dispositivo; publicar o site não transfere os dados de um celular para outro.

## Arquivos

- `index.html`: aplicação publicada no GitHub Pages.
- `BuzzDataBase.html`: cópia idêntica da aplicação.
- `sw.js`: cache/offline do PWA com versão atualizada.
- `manifest.webmanifest` e ícones: instalação como aplicativo.
