# Compras do Sábado: app para Android

Calculadora de compras de supermercado com limite de gasto (opcional), várias calculadoras ao mesmo tempo,
pré-lista, histórico por data e cópia de segurança. Funciona **sem internet** e guarda os dados **só no seu aparelho**.
Não tem conta, login nem envio de dados para lugar nenhum.

## Como colocar no ar (uma vez só)

O Chrome só instala o app se ele estiver num endereço seguro (https). Por isso a pasta precisa ser publicada.
Escolha UMA das opções abaixo. As duas são gratuitas. Os nomes dos menus podem mudar com o tempo.

### Opção A: Netlify Drop (a mais rápida, sem programar)
1. No computador, abra https://app.netlify.com/drop
2. Arraste a pasta **compras-do-sabado** (inteira) para a área indicada.
3. O site publica na hora e mostra um endereço (algo como `nome-aleatorio.netlify.app`).
4. Crie uma conta gratuita quando ele pedir, para o endereço não expirar.

### Opção B: GitHub Pages
1. Crie uma conta em https://github.com e um repositório **público** novo (ex.: `compras`).
2. Em **Add file → Upload files**, envie os arquivos de dentro da pasta (index.html, sw.js, manifest.webmanifest e os 3 ícones) e confirme (**Commit**).
3. Vá em **Settings → Pages**, escolha **Deploy from a branch**, branch **main**, pasta **/ (root)** e salve.
4. Após 1 ou 2 minutos, o endereço fica em `https://SEU-USUARIO.github.io/compras/`.

O repositório público só contém o código do app. Nenhum dado seu vai para lá.

## Como instalar no Android
1. Abra o endereço no **Chrome** do celular, com internet, e deixe a página carregar por completo.
2. Toque no botão **📲 Instalar no celular** que aparece na tela inicial do app. Se ele não aparecer, toque nos três pontinhos (⋮) do Chrome e escolha **Instalar app** (ou **Adicionar à tela inicial**).
3. O ícone do carrinho aparece na tela do celular. A partir daí, abre em tela cheia e funciona no modo avião.

## Seus dados
- Ficam guardados dentro do aparelho. Se você **limpar os dados do app/Chrome** ou **trocar de celular**, eles se perdem.
- Por isso existe a **Cópia de segurança** na tela inicial:
  - **Salvar cópia** baixa um arquivo `compras-copia-AAAA-MM-DD.json`. Guarde no Google Drive, no WhatsApp ou envie por e-mail.
  - **Restaurar cópia** carrega esse arquivo em qualquer aparelho (substitui os dados que estiverem lá).
- Cada pessoa (você e sua mãe) tem os próprios dados no próprio celular, sem sincronizar.
- Os dados da versão que você testou no Claude **não passam sozinhos** para este app. O que for importante, digite de novo.

## Como atualizar o app depois
Substitua os arquivos no mesmo endereço (Netlify: arraste a pasta de novo no mesmo site; GitHub: envie os arquivos de novo).
O celular pega a versão nova em uma ou duas aberturas do app com internet. Os dados não se perdem.

## Arquivos
- `index.html`: o app inteiro
- `manifest.webmanifest`: nome e ícones do app instalado
- `sw.js`: faz o app funcionar sem internet
- `icon-*.png`: ícones
