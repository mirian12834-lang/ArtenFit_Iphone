# Meu Treino — versão para iPhone e Android (PWA)

Esta pasta contém o site do Meu Treino preparado para ser instalado na tela inicial do iPhone como um app da web (PWA). Os exercícios, as cargas e o tema são salvos no `localStorage` do navegador. O `service worker` armazena os arquivos do app para permitir reabertura offline depois que ele foi carregado uma primeira vez.

## Importante

Para instalar como app na tela inicial e ativar o modo offline, publique todos os arquivos desta pasta em um endereço HTTPS. Abrir `index.html` diretamente pelo app Arquivos não ativa os recursos completos de instalação/offline.

## Publicar com GitHub Pages

1. Entre em https://github.com e crie um repositório novo, por exemplo `meu-treino`.
2. Envie **todos os arquivos e pastas que estão dentro desta pasta**, incluindo `index.html`, `manifest.webmanifest`, `sw.js` e `icons/` (não envie apenas o ZIP).
3. No repositório, abra **Settings → Pages**.
4. Em **Build and deployment**, escolha **Deploy from a branch**; selecione a branch `main` e a pasta `/(root)`, depois clique em **Save**.
5. Aguarde o GitHub Pages publicar e abra o endereço HTTPS que ele indicar. A URL costuma ter o formato `https://SEU-USUARIO.github.io/meu-treino/`.

## Instalar no iPhone

1. Abra a URL publicada no **Safari** do iPhone.
2. Toque em **Compartilhar**.
3. Selecione **Adicionar à Tela de Início**.
4. Confirme o nome “Meu Treino” e toque em **Adicionar**.
5. Abra o ícone criado na tela inicial. Abra o app pelo menos uma vez com internet para que os arquivos offline sejam armazenados.

## Atualização

Após publicar alterações nos arquivos, feche/reabra o app com internet. Como os arquivos estáticos ficam em cache, em alguns casos pode ser necessário fechar o app e abrir novamente para receber a versão atualizada.

## Dados

Os treinos ficam no armazenamento local daquele iPhone/origem. Eles não sincronizam automaticamente com o Android ou outros aparelhos. Evite apagar os dados do site ou remover o app sem antes exportar/anotar cargas importantes; o `localStorage` não é um backup em nuvem.
