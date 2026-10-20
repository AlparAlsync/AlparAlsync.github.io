# Alsync · site do produto

SPA estática de divulgação do **Alsync**, produto de expurgo e arquivamento de dados desenvolvido pela Alpar.

## Arquivos

| Arquivo | Para que serve |
| --- | --- |
| `index.html` | O site completo (HTML, CSS e JS em um único arquivo) |
| `favicon.svg` | Ícone da aba do navegador |
| `.nojekyll` | Faz o GitHub Pages servir os arquivos como estão, sem processar com Jekyll |

Não há build nem dependências. As fontes (Archivo, IBM Plex Sans e IBM Plex Mono) vêm do Google Fonts.

## Navegação

- `#inicio`: página principal, em um único scroll
- `#como-funciona`, `#seguranca`, `#indicadores`, `#implantacao`, `#midia`: atalhos para as seções da página principal
- `#contato`: página de contato

## Publicar no GitHub Pages

1. Copie os arquivos para a raiz do repositório (ou para a pasta `/docs`).
2. Em **Settings → Pages**, em **Build and deployment**, escolha **Deploy from a branch** e selecione a branch e a pasta.
3. Para um repositório `<org>.github.io`, o site fica em `https://<org>.github.io/`.

## Pendências antes de ir ao ar

- **Cores da marca:** `--brand` e `--brand-2` no topo do `<style>` são provisórias. Substitua pelos hex oficiais da Alpar.
- **Logo:** hoje a marca aparece só em texto ("Alsync by Alpar").
- **Fotos e vídeos:** a seção `#midia` tem espaços reservados. Para usar um vídeo, coloque o MP4 em `assets/` e troque o bloco `.slot` por `<video controls src="assets/arquivo.mp4"></video>`.
- **Formulário de contato:** só valida os campos e mostra uma mensagem; não envia nada. Para receber os contatos, ligue o `submit` a um serviço de formulários ou a uma API da Alpar.
- **Números e textos:** os KPIs, o gráfico e o log de execução usam dados de exemplo. Os textos de segurança devem ser validados com a equipe do produto.
