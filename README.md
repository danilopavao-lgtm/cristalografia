# Cristalografia de proteínas em simulações

Conjunto de simulações interativas para estudo de cristalografia de proteínas, do conceito de série de Fourier até o refinamento do modelo.

## Simulações

1. Série de Fourier e derivada espectral
2. Fatores de estrutura e síntese de densidade (1D)
3. Do padrão de difração ao modelo (2D)
4. Estatísticas de processamento por camada de resolução
5. Substituição molecular
6. Aparência do mapa em função da resolução
7. Refinamento: mapas de diferença e Rfree

## Estrutura

- `index.html`: página inicial com o roteiro.
- `01-…html` a `07-…html`: uma página por simulação, cada uma independente.
- `estilo.css`: estilo comum (modo claro e escuro automáticos).
- `.nojekyll`: faz o GitHub Pages servir os arquivos sem processamento.

O site é HTML/JS puro, sem etapa de build. As únicas dependências externas, carregadas por CDN, são o Chart.js (gráficos) e a fonte de ícones Tabler.

## Publicar no GitHub Pages

1. Crie um repositório no GitHub (por exemplo, `cristalografia-simulacoes`).
2. Envie todos os arquivos desta pasta para a raiz do repositório (inclusive o `.nojekyll`).
3. Em **Settings → Pages**, em *Build and deployment*, escolha **Deploy from a branch**, branch `main`, pasta `/ (root)`.
4. Após alguns minutos, o site fica disponível em `https://<usuario>.github.io/cristalografia-simulacoes/`.

Para testar localmente, basta abrir o `index.html` no navegador, ou rodar `python3 -m http.server` nesta pasta e acessar `http://localhost:8000`.
