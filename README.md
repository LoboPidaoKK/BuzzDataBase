# BuzzDataBase — pacote pronto para GitHub Pages

Esta versão mantém o visual, as funções de edição, importação/exportação de backup e os 10 tópicos iniciais, sem obras cadastradas. Ao tocar em uma capa disponível, ela abre em visualização ampliada; feche tocando no X, fora da imagem ou pressionando Esc. Ao salvar uma edição ou adicionar uma obra, o site mantém o tópico/filtros atuais e tenta preservar a posição de rolagem. **Os três ícones ficam na raiz**, junto com `index.html`; não é necessário criar nem enviar uma pasta `icons`.

## Arquivos principais

- `index.html`: página inicial usada pelo GitHub Pages.
- `BuzzDataBase.html`: cópia da página para abertura direta.
- `icon-180.png`, `icon-192.png`, `icon-512.png`: ícones do navegador e do app, todos na raiz.
- `buzzdatabase-icon.png`: imagem original do ícone.
- `manifest.webmanifest`: configuração de instalação como aplicativo web.
- `sw.js`: cache da estrutura básica para uso offline após o primeiro carregamento.

## Publicar no GitHub Pages pelo celular

1. Extraia este ZIP no celular.
2. No repositório `BuzzDataBase`, envie **os arquivos que estão dentro do ZIP** para a primeira tela do repositório (raiz). Não envie o ZIP como substituto dos arquivos e não coloque tudo dentro de uma pasta extra.
3. Se o GitHub perguntar se deseja substituir arquivos existentes, confirme para atualizar a versão.
4. Em **Settings → Pages**, selecione **Deploy from a branch**, branch `main` e pasta `/(root)`, e salve.
5. Aguarde a publicação. O site fica em `https://lobopidaokk.github.io/BuzzDataBase/`.

## Baixar o site pelo GitHub

Depois de enviar estes arquivos ao repositório, o ZIP completo pode ser baixado pelo link abaixo (ele acompanha a versão atual da branch `main`):

https://github.com/lobopidaokk/BuzzDataBase/archive/refs/heads/main.zip

O site publicado também tem um link **“Baixar o BuzzDataBase (ZIP)”** no rodapé.

## Uso e backups

- As obras, categorias e favoritos ficam salvos no navegador/dispositivo usado; não sincronizam automaticamente entre aparelhos.
- Use **Exportar backup** para salvar o catálogo em JSON e **Importar backup** para recuperá-lo.
- Capas automáticas dependem de internet; imagens enviadas manualmente ficam no armazenamento local desse navegador.
- Publicar um repositório significa deixar seu código visível. Não coloque senhas, tokens ou dados privados nele.
