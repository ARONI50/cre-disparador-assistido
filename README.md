# CRE — Disparador Assistido PWA v0

Este é um campo de teste isolado. Ele não mexe na Central de Trabalho.

## O que ele faz

- Salva mensagem no próprio aparelho.
- Salva contatos no próprio aparelho.
- Mostra um contato por vez.
- Abre o WhatsApp com a mensagem pronta.
- Você confirma manualmente o envio.
- Depois volta e marca como ENVIADO ou PULAR.
- Gera relatório TXT.

## O que ele NÃO faz

- Não envia mensagem sozinho.
- Não usa robô.
- Não burla WhatsApp.
- Não depende da planilha.
- Não mexe na Central de Trabalho.

## Como testar no computador

1. Descompacte o arquivo ZIP.
2. Abra `index.html` no navegador.
3. Cadastre 1 ou 2 contatos de teste.
4. Clique em Disparo.
5. Clique em Abrir WhatsApp.

## Como testar melhor como PWA

Para instalar como aplicativo, hospede a pasta em:
- GitHub Pages
- Firebase Hosting
- Netlify
- Vercel

Depois abra pelo celular e use "Adicionar à tela inicial".

## Firebase depois

A versão v0 usa `localStorage`, ou seja, salva no próprio aparelho.

Depois da aprovação, a versão v1 pode usar Firebase:
- Firebase Hosting para hospedar o PWA.
- Firestore para contatos, mensagens e logs.
- Firebase Authentication se precisar login.

## Estrutura

- `index.html`: aplicativo completo
- `manifest.json`: instalação como PWA
- `service-worker.js`: cache/offline básico
- `icon.svg`: ícone do app
