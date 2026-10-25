# BuzzDataBase — instalação e GitHub Pages

Este pacote contém uma versão preparada para funcionar como PWA (aplicativo web instalável).

## Arquivos
- `index.html`: entrada principal, usada automaticamente pelo GitHub Pages.
- `BuzzDataBase.html`: cópia com nome explícito, útil para abrir diretamente.
- `manifest.webmanifest`: nome, cores, ícones e configuração do PWA.
- `sw.js`: service worker para abrir a estrutura principal offline após o primeiro carregamento.
- `icons/`: ícones da aba do navegador e do app, derivados da imagem enviada.
- `buzzdatabase-icon.png`: imagem original enviada.

## Publicar no GitHub Pages
1. Entre no GitHub e crie um repositório chamado **BuzzDataBase**.
2. Envie os arquivos e a pasta `icons` para a **raiz** do repositório (não coloque tudo dentro de uma pasta extra).
3. Abra **Settings → Pages**.
4. Em **Build and deployment**, selecione **Deploy from a branch**.
5. Escolha a branch `main` e a pasta `/(root)`, depois clique em **Save**.
6. Aguarde o GitHub publicar e abra o endereço indicado nessa página. Para um repositório chamado `BuzzDataBase`, normalmente será `https://SEU-USUARIO.github.io/BuzzDataBase/`.

## Instalar no Android
1. Abra o endereço publicado no Chrome usando HTTPS e carregue o site uma vez com internet.
2. Toque em **Instalar** no próprio site, se o botão de instalação estiver disponível, ou abra o menu `⋮` do Chrome.
3. Escolha **Instalar app** ou **Adicionar à tela inicial**.

A disponibilidade do botão de instalação depende do navegador. Em alguns aparelhos, é necessário usar o menu do navegador.

## Observações importantes
- O PWA e o service worker exigem HTTPS (o GitHub Pages fornece HTTPS) ou `localhost`; não são ativados ao abrir o arquivo via `file://`.
- A estrutura principal pode abrir offline após carregar e instalar/cachear os arquivos, mas capas automáticas que dependem de serviços externos precisam de internet.
- A coleção e os favoritos ficam salvos no armazenamento local daquele navegador/dispositivo. Não são sincronizados automaticamente entre você e seu amigo.
- Use **Exportar backup** no site para guardar sua coleção em JSON. Não limpe os dados do navegador sem antes fazer backup.
- Ao publicar num repositório público, qualquer pessoa pode ver o código do site. Não coloque senhas, tokens ou informações privadas nele.

## Atualizar depois
Envie os arquivos atualizados ao mesmo repositório. Se uma versão antiga ficar em cache, feche e reabra o app com internet; o service worker atualizado trocará a versão do cache.

## Gerenciar tópicos
- Use **🗂️ Gerenciar tópicos** para criar, renomear e excluir categorias.
- Você pode criar, por exemplo, **Mangás**, **HQs**, **Jogos Zerados**, **Jogos Vistos**, **Livros** ou quantas categorias quiser.
- Renomear um tópico atualiza todas as obras daquela categoria.
- Se excluir um tópico que contém obras, você pode digitar o nome de outro tópico para transferi-las ou deixar a resposta em branco para mantê-las sem tópico. Cancelar a janela interrompe a exclusão. Obras sem tópico continuam na coleção em “Tudo” e podem ser categorizadas novamente ao editar.
- Os backups agora guardam também a lista de tópicos vazios; backups antigos continuam podendo ser importados.


## Coleção reorganizada
A versão inicial vem separada em Anime, YouTube, DC, Marvel, Star Wars, Desenhos, Filmes e Séries, itens que você não recomenda, Atores e Games Zerados. As capas não foram preenchidas para que você possa adicioná-las depois.

### Visualização das capas
Clique ou toque em qualquer capa disponível para abri-la ampliada sobre um fundo escuro. Feche pelo botão ×, tocando fora da imagem ou pressionando Esc no teclado.
