# Cartinha NFC 💙

Site estático preparado para ser publicado na internet e aberto por um cartão NFC.

## Estrutura

- `index.html` — página completa da cartinha, com HTML/CSS/JavaScript e imagens incorporadas.
- `.nojekyll` — evita processamento desnecessário pelo Jekyll quando usado no GitHub Pages.
- `LEIA-ME-NFC.txt` — guia rápido para publicação e gravação do NFC.

## Publicação

O projeto não precisa de Node.js, banco de dados ou build. Basta publicar o conteúdo desta pasta em uma hospedagem de arquivos estáticos.

### GitHub Pages

1. Crie um repositório no GitHub.
2. Envie `index.html`, `.nojekyll`, `README.md` e `LEIA-ME-NFC.txt` para a raiz do repositório.
3. Em **Settings → Pages**, selecione **Deploy from a branch**, branch `main` e pasta `/(root)`.
4. Salve e aguarde a publicação.
5. Copie a URL HTTPS fornecida pelo GitHub Pages.

O `index.html` já está na raiz, como esperado pelo GitHub Pages.

## NFC

Depois que a URL estiver pública, grave **somente a URL HTTPS** na tag/cartão NFC usando um registro NDEF do tipo URL.

O cartão não precisa conter os arquivos do site: ele funciona como um atalho para a página hospedada.

## Experiência NFC

Ao carregar a página, a versão atual inicia automaticamente a sequência da cartinha após um pequeno intervalo. O controle manual continua disponível como alternativa caso a reprodução automática seja limitada pelo navegador.

## Observação

O celular pode mostrar uma notificação ou pedir uma ação antes de abrir o link NFC. Isso depende do sistema operacional e das configurações do aparelho; o site não consegue eliminar essa etapa.
